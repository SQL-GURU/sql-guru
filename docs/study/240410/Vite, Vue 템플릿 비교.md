```
pnpm create vite@latest my-vite-vue --template vue
```

```
pnpm create vue@latest my-vite-vue
```

두 커맨드 모두 Vite + Vue 기본 프로젝트 구조를 만들어줌

### `create vite`

- Vite 을 사용하는데 필수적인 최소한의 설정만 해줘서 Vite 을 이해하는데 더 도움이 됨
  - Vite 은 Framework-Agnostic (프레임워크에 구애받지 않음) 를 추구함

### `create vue`

- Vue 를 사용하는데 필요한 부가적인 옵션을 커맨드라인에서 쉽게 적용할 수 있음
  - ESLint, Prettier, Vitest 등
 
## TIL

Vite 기본과 Vue 기본을 비교하면서 나만의 기본을 만들어 보는 재미가 있다.

예를 들어 둘 다 기본 CSS 를 제공해주는데 디테일이 약간 달라서 두 개를 입맛대로 Merge 하면 손쉽게 현대적인 기본 CSS 를 만들 수 있다.

그렇게 해서 합쳐 본 것

```css
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  font-weight: normal;
}

:root {
  font-family:
    Inter,
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    Oxygen,
    Ubuntu,
    Cantarell,
    'Fira Sans',
    'Droid Sans',
    'Helvetica Neue',
    sans-serif;
  line-height: 1.6;
  font-size: 18px;

  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
```

내가 처음부터 만든 것과 요즘 느낌 나는 현대적인 앱을 보면 미세하게 어딘가 다른 느낌이 나는데

(내꺼는 묘하게 짜치고 요즘꺼는 묘하게 세련됨)

요즘 느낌 나는 앱들은 `text-rendering: optimizeLegibility;` 등 폰트 랜더링에 많이 신경 쓰는 것을 알 수 있다.
e.g. https://vitejs.dev (Vite 공식)
