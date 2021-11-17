---
title: Flutter push 개발기
tags: [Flutter, blog, Firbase]
style: 
color: 
description: Flutter Push Notifications
---

### 1. 플러그인 설치
- firebase_core: ^1.8.0
- firebase_messaging: ^10.0.9
- flutter_local_notifications: ^9.0.2

일단, 이전에 flutter를 사용하여 만든 웹앱이 있었다. (내 p;ㅠ)
해서 처음에는 firebase를 사용할건지 말건지에 대해서 조금 고민을 했었는데, 아무래도 조금 더 편하게 작업할 수 있는 firebase를 사용하여 푸시를 구현하기로 하였다.
그래서 작업기준일(2021.11.01 가장 최신의 플러그인들을 저렇게 설치 해 주었다.


### 2. ios Setting
나의 경우에는 이미 firebase analysis를 연결한 상태고
처음 어플을 만들때 Push Notifications에 체크도 해주었기 때문에 별도로 설정할 부분은 크게 없었다.
하지만 순서를 지정해보자면, 일단 애플의 Identifiers 에서 App ID, Bundle ID를 확인.
Push notifications를 위한 keys를 생성하여 firebase의 해당 앱에 APN 인증 키를 업로드 해야한다.
해당 키를 업로드 하고나면 firebase에서 GoogleService-info.plist를 다운받아 내 앱 Runner에 등록해준다 

다만, 내 앱은 실제 배포되는 앱과 개발앱의 Bundle ID가 달라서 GoogleService-info.plist를 두개 만들어서 xcode에서 Build Phases 에 Google plist라는 스크립트를 생성한 후 
프로젝트 빌드 기준에 따라 (나는 Debug, Release 모드 두개만 사용했다) 원하는 파일 내용이 GoogleService-info.plist에 설정되도록 작업해 주었다. 


그리고 소스에서는 
ios/Podfile 에 platform :ios, '10.0'를 삽입해주고 cocoaPod를 새로 설치해 주었다.


### 3. android Setting
1. android/app/build.gradle 에 
    implementation 'com.google.firebase:firebase-messaging'
를 넣어주었다.

2. AndroidManifest.xml에 
  <meta-data
      android:name="com.google.firebase.messaging.default_notification_channel_id"
      android:value="value" // 앱이름으로 설정했음
  />
를 추가했다.

3. /android/app/src/main/res/drawable/app_icon.png 푸시 받을때 표시될 앱 아이콘을 추가해줌


### 4. 소스작성
소스의 경우에는 따로 작업해서 올려놓도록 하겠다.
나는 어떤 분의 소스를 참조하여 작업하였으며 
getX를 통해서 상태관리 형태로 작업했다. 

내가 염두하고 작업한 부분은 아래와 같다.
1. background, foreground에 있어도 head에 푸시형태로 나타날것
2. 이미지 전달이 가능할 것
3. ios, android에서 동일하게 동작할 것

