---
name: Mediance UI
tools: [React]
image: 
description: 통일된 우리(mediance)만의 UI framework
align: 1
---

## Mediance UI

**1. 기간**   
2022-06 ~ 2022-10  
  
**2. 사용기술, 툴 및 환경**   
- `React.js(vite)`, `HTML`, `SCSS`, `storybook`
- `git(gitlab)`
  
**3. 기여도**   
100%

**4. 성과 및 문제해결**
- 최초작업 시에는 `Lit`을 사용하려 작업하여 프레임워크에 상관없이 사용할 수 있도록 하려고 했으나 컴포넌트안에 slot은 사용되지만 데이터를 binding 하는데 slot안으로는 데이터 전달이 어려워 `React`로 작업하게 됨.
- 지정 디렉토리만 접근하도록 하기 위해 exports에 `path`를 지정해 줬고, `Chunks`파일 정리를 위해 rollup manualChunks 설정 추가함.