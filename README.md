# Prettier 사용하기

**[👉🏻 Prettier 공식문서 👈🏻](https://prettier.io/docs/en/)**

## 0️⃣ Overview

- Prettier는 설치형 소프트웨어
- 아래의 명령어로 프로젝트 내에 Prettier를 설치
  - `npm install -D prettier`
  - 또는 `yarn add -D prettier`
- 프로젝트 내에 설치한 `prettier`를 실행함으로써 코드를 포맷팅
  - `package,json` 내 `scripts`에 실행 커맨드 작성 후 실행
  - 또는 터미널에서 `npx prettier` 명령어를 바로 입력 후 실행
- 프로젝트의 root에 `.prettierrc.js`와 같은 설정 파일을 생성하여 사용

---

## 1️⃣ Installation

프로젝트 내에서 아래의 명령어를 실행하여 **`prettier`** 패키지를 `devDependency`로 `node_modules`에 설치

- `npm install -D prettier`
- 또는 `yarn add -D prettier`

---

## 2️⃣ Usage

프로젝트 내에 설치한 `prettier`를 아래와 같은 방법으로 실행함으로써 코드를 포맷팅

#### [옵션 1]

1. `package.json` 내 `scripts`에 다음과 같이 추가

   ```javascript
   "format": "prettier . --write"
   ```

2. 터미널에 아래의 명령어를 입력하여 `format` 커맨드를 실행

- `npm run format`
- 또는 `yarn format`

#### [옵션 2]

1. 터미널에 `npx prettier . --write`를 입력 후 실행

---

## 3️⃣ Configuration

1. 아래의 형태 중 하나를 선택하여 프로젝트 루트에 파일 추가

- A "prettier" key in your package.json file. (파일 추가 X)
- A .prettierrc file written in JSON or YAML.
- A .prettierrc.json, .prettierrc.yml, .prettierrc.yaml, or .prettierrc.json5 file.
- A .prettierrc.js, or prettier.config.js file that exports an object using export default or module.exports (depends on the type value in your package.json).
- A .prettierrc.mjs, or prettier.config.mjs file that exports an object using export default.
- A .prettierrc.cjs, or prettier.config.cjs file that exports an object using module.exports.
- A .prettierrc.toml file.

**아직 작성 중**

<!--
## Workspace(작업 공간) Settings

```javascript
{
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.codeActionsOnSave": {
    "source.organizeImports": "explicit"
  },
}
``` -->
