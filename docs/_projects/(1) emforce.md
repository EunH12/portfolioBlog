---
name: eMFORCE Homepage
tools: [Vue, three.js, HTML, SCSS]
image: https://eunh12.github.io/portfolioBlog/assets/img/emforce_title.png
description: eMFORCE 홈페이지 리뉴얼 (반응형)
align: 1
---

## eMFORCE Homepage
![](https://eunh12.github.io/portfolioBlog/assets/img/emforce_title.png)

**1. 기간**   
2020-07 ~ 2020-09   
  
**2. 사용기술, 툴 및 환경**   
- `Vue(vue-cli)`, `Vuex`, `Rest API`, `Axios`, `three.js`, `masonry`, `gsap`, `HTML`, `SCSS`  
- `git(AWS CodeCommit)`, `AWS(S3/CloudFront)`
  
**3. 기여도**   
100%   

**4. 성과 및 기타사항**   
- 사내 3d 기술 최초 구현 및 도입, 팀 내 기술 공유  
- 메인페이지 우주화면 구현을 위하여 `three.js`를 사용하여 별 및 우주 공간 3d 형태로 구현. (배경은 큐브형태의 3d화면, 별은 2d 형태의 geometry로 서로 다른 방향으로 이동하여 조금 더 입체적인 느낌이 나도록 구현)  
- explorer 에서 object-fit 미지원으로 영상 화면 fix, 3d(webGL) 미 지원으로 우주화면 정적인 이미지로 변경 및 안내문구 추가  
- `gsap`내 ScrollTrigger, Stagger 등을 사용한 애니메이션 효과   
- `masonry`를 사용해 핀터레스트 화면 구현 (데이터를 불러올때 이미지 로딩이 사용자 별로 달라 해당 레이아웃이 깨지는 현상 발생하여 `vue-images-loaded`를 추가하여 로딩 후 작동 하도록 변경함)   
- 포트폴리오 내부 팝업 슬라이드 ( swiper 사용하였으나 센터 정렬 등의 디자인 구현이 되지 않아 slick으로 변경. 하지만 slick의 beforeChange 등의 event가 정확하게 동작하지 않아 vue 내부의 data로 저장하고 저장된 data 기준으로 슬라이더의 인터렉션 작업.)  
- pdf 오픈 문제 : 어떤 부분에서는 파일이 웹상에서 오픈되고 어떤 부분에서는 다운로드 되는 문제가 있어 확인해본 결과 s3 contents-type의 문제로 어드민에서 등록시 binary가 아닌 application/pdf 로 변경하여 저장하도록 함.
   
<br>    
<br>    
      

**5. 화면 상세**   
![](https://eunh12.github.io/portfolioBlog/assets/img/emforce_content.png)  
![](https://eunh12.github.io/portfolioBlog/assets/img/emforce_content2.png)  
   
**6. 링크**   
[go to Site](https://dbvz3778s760x.cloudfront.net/){: target="_blank"}
