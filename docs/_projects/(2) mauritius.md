---
name: 굿초보 3.0
tools: [Vue, Nuxt.js]
image: https://eunh12.github.io/portfolioBlog/assets/img/Mauritius_title.png
description: 기존 굿초보 사이트에서 상품판매에 특화된 사이트
---

## 굿초보 3.0  
![](https://eunh12.github.io/portfolioBlog/assets/img/Mauritius_title.png)  
  
**1. 기간**   
2020-02 ~ 2020-05   
  
**2. 사용기술 및 툴**   
`Vue`, `Nuxt.js`, `HTML`, `SCSS`, `storybook`, `antdesign`  
  
**3. 기여도**   
클라이언트 프론트(30%) / 어드민 프론트 (50%)   
   
**4. 기타 사항**   
* 프론트: 상품 구매 후 프로세스 담당 ( 구매확인, 환불 등 )
  - 기본 모바일 페이지로 구성되어 있어 pc 화면에서도 모바일 화면처럼 보이고 레이아웃만 반응형인 사이트
  - 네이버 SEO 최적화를 위하여 `Nuxt.js`를 통한 SSR   
  - 컴포넌트 자체 제작으로 해당 컴포넌트 관리를 위해 `storybook` 도입  ( 직접 작업한 컴포넌트 : 클릭버튼, 드롭다운, 리스트카드, svgicon, fixedbutton 등)
* 어드민 프론트 : 회사관리, 구매관리, 쿠폰관리 담당
  - 디자인 없이 `antdesign` UI framework 사용
  - 작업중 쿠폰관리의 경우 쿠폰을 상품에 연결을 해야하는 작업이 조금 어려웠다, 상품 판매계약별로 쿠폰을 다르게 지정 할수있어서 상품 리스트를 불러와 상품 판매계약을 정렬하고 판매계약별 세부 리스트를 체크해서 그 상품에 쿠폰을 등록하는 형태였다. 때문에 상품을 체크한 리스트배열, 판매계약별로 쿠폰을 지정한 리스트배열을 따로 지정하였고, 팝업으로 구성되어있어 부모창의 배열을 복사해 새로 지정하고 변경체크 후 최종 반영까지 진행 하였는데 두가지 배열이 상호 작용을 하다보니 좀 어려웠던 것 기억이 있다.

      
<br>    
<br>     

**5. 화면 상세**   
![](https://eunh12.github.io/portfolioBlog/assets/img/Mauritius_con.png)  
![](https://eunh12.github.io/portfolioBlog/assets/img/Mauritius_con2.png)  
   
**6. 링크**  
[go to Site](http://insurance.goodchobo.com/){: target="_blank"}
