# OSS Week 12 — React Hooks Playground (Student Starter)

## 실행 방법
Node.js 20.19+ 또는 22.12+ 권장. 프로젝트 폴더에서 실행:

```bash
npm install
npm run dev
```

브라우저에 터미널의 Local URL을 열고 LAB 탭을 이동하세요. 제출 전 `npm run build`도 실행하세요.

## 수행 방법
1. `src/components/` 아래의 LAB 1~4 파일에 있는 `TODO`를 직접 완성합니다.
2. `src/App.jsx`, `src/App.css`는 공통 화면이므로 가급적 수정하지 않습니다.
3. 각 LAB의 동작 화면과 콘솔 결과를 기록합니다.
4. 한 LAB에서 다른 LAB으로 탭을 전환하면 기존 컴포넌트가 언마운트됩니다. Cleanup 결과를 관찰합니다.


## 이해도 확인 질문
1. useEffect의 Dependency Array가 필요한 이유는?  
- useEffect 내부 코드 실행 타이밍을 제어하고, 불필요한 재실행 및 무한 루프를 방지하기 위해서 필요함.
2. Cleanup을 사용하지 않으면 어떤 문제가 발생할 수 있는가?  
- 타이머가 중복으로 실행되는 문제가 발생할 수 있음.
3. useState와 useRef의 가장 중요한 차이는?  
- 값을 변경할 때 컴포넌트가 화면을 갱신하는지 아닌지. useState는 화면에 즉시 반영, useRef는 리렌더링을 일으키지 않음.
4. LAB 2와 LAB 4의 Timer 관리 방식은 어떻게 다른가?  
- 타이머 관리가 다른데, lab2는 useEffect 기반으로 관리, lab4는 useRef 기반으로 관리함.
