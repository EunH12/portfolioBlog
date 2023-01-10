---
name: Mediance Site + App
tools: [Vue, Flutter]
image: https://eunh12.github.io/portfolioBlog/assets/img/mediance_main.png
description: 미디언스 사용자 홈페이지 리뉴얼 프로젝트(반응형) / 웹뷰 앱
align: 1
---

## Mediance Homepage
![](https://eunh12.github.io/portfolioBlog/assets/img/mediance_main.png)


**1. 기간**   
2021-03 ~ 2022-10  
  
**2. 사용기술, 툴 및 환경**   
- `Vue(vite)`, `Pinia`, `Rest API`, `Axios`, `flicking`, `gsap`, `HTML`, `SCSS` , `Flutter` 
- `git(github)`, `Vercel`, `x-code`
  
**3. 기여도**   
site: 70%, app: 50%

**4. 성과 및 문제해결**
사이트:
- 체험 신청 후 진행 프로세스 / 포인트 / 개별 회원 소셜미디어 채널 통계 부분 개발
- `vue.js2.0 + vue cli + vuex` => `vue 3.0 + vite + pinia` 로 변경
- 웹폰트를 내부 폰트로 사용할 시 리소스 및 로딩 문제가 있고 구글폰트의 경우도 가끔 로딩이슈가 있어, 웹폰트 로딩 안될시 내부폰트 이용하는 식으로 개선함.

앱:
- 자연스러운 네비게이션을 위해 네비게이션은 네이티브로 작업 후 작동은 사용자 사이트에 해당 스크립트를 심고 `evaluateJavascript`로 실행.
- 로그인 페이지를 통합로그인 사이트로 변경 하면서 로그인이 유실되는 이슈가 생겨, token을 다른 controller에 저장 및 추가하여 해결.
- 페이스북 로그인시 임베디드 브라우저 로그인 작동 불가한 이슈가 있어, 외부브라우저로 이동 시킨 후 앱으로 돌아와 다시 로그인을 확인하는 브릿지 추가하여 해결.
<br>    
      

**5. 화면 상세**   
![](https://eunh12.github.io/portfolioBlog/assets/img/mediance_content1.png)  
![](https://eunh12.github.io/portfolioBlog/assets/img/mediance_content2.png)  
   
**6. 링크**   
[go to Site](https://app.mediance.co.kr){: target="_blank"}
