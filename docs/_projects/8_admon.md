---
name: ADmon
tools: [Vue, antdesign]
image:
description: 네이버 타임보드 데이터 수집 사이트
align: 8
---

## ADmon

**1. 기간**   
2019-10 ~ 2019-11  
  
**2. 사용기술, 툴 및 환경**   
- `Vue(vue-cli)`, `Vuex`, `Rest API`, `Axios`, `antdesign`, `HTML`, `SCSS`
- `git(AWS CodeCommit)`, `AWS(S3/CloudFront/Cognito)`  
  
**3. 기여도**   
80%   
   
**4. 성과 및 문제해결**
- 별도의 테스트 서버 존재하지 않아, `netlify` 사용하여 테스트 화면 구현  
- 기존의 타 프로젝트에 존재하던 `AWS Cognito` 기반의 회원에게 권한을 부여하는 형태로, 새로운 그룹에 추가하는 형식으로 로그인 개발 (회원가입 불가, 기존 UserPool에서 데이터 확인, 해당 그룹에 있는지 판단, 그룹 추가 후 로그인 가능)  

      
      