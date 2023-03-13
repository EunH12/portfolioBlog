---
name: Mediance UI(미완성)
tools: [React]
image: 
description: 매번 UI를 새로 개발하는 것보다 통일된 우리(mediance)만의 UI components library 가 있으면 좋겠다고 생 각하여 작업.
align: 3
---

## Mediance UI

**1. 기간**   
2022-06 ~ 2022-10  
  
**2. 사용기술, 툴 및 환경**   
- `React.js(vite)`, `HTML`, `SCSS`, `storybook`
- `git(gitlab)`
  
**3. 기여도**   
100% (미완성이며 릴리즈 하진 않았음)

**4. 성과 및 문제해결**
- 최초작업 시에는 `Lit`을 사용하려 작업하여 프레임워크에 상관없이 사용할 수 있도록 하려고 했으나 컴포넌트안에 slot은 사용되지만 데이터를 binding 하는데 slot안으로는 데이터 전달이 어려워 `React`로 작업하게 됨.
- 지정 디렉토리만 접근하도록 하기 위해 exports에 `path`를 지정해 줬고, `Chunks`파일 정리를 위해 rollup manualChunks 설정 추가함.

**5. 링크**   
[go to Site](https://github.com/EunH12/exUi){: target="_blank"}