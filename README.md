# 리액트 프로젝트 생성

## 최신버전의 리액트 프로젝트 생성

```js
npx create-react-app 프로젝트이름
```

## 17버전으로 다운그레이드 하기

vscode에서 터미널을 열고 다음과 같이 react, react-dom을 17버전으로 재설치

```js
npm i react@17 react-dom@17 --save
```

## 리액트 라우터는 5버전대 설치

vscode에서 터미널을 열고 다음과 같이 react-router-dom을 5버전으로 재설치

```js
npm i react-router-dom@5 --save
```

## sass 설치

vscode에서 터미널 열고 다음의 명령어로 sass 설치

```js
npm i sass --save
```

---

# 리액트 프로젝트 폴더 정리

## 다음의 이미지와 같이 불필요한 파일 삭제

![폴더구조](https://cafeptthumb-phinf.pstatic.net/MjAyMjA1MDJfMTE2/MDAxNjUxNDc2OTg2OTY0.kegR8AAuOOLZvUQwq3v1KnmjrgTi3f67Es8_R58wxeYg.NT3ze0yKW9Rt00rhG2ENttvRg40I-wY6QIL6COnMe4Eg.PNG/image.png?type=w1600)

## 각 파일 코드 수정

public 폴더 안쪽의 index.html 다음과 같이 수정

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="utf-8" />
		<link rel="icon" href="%PUBLIC_URL%/favicon.ico" />
		<meta name="viewport" content="width=device-width, initial-scale=1" />
		<title>React App</title>
	</head>
	<body>
		<noscript>You need to enable JavaScript to run this app.</noscript>
		<div id="root"></div>
	</body>
</html>
```

src 폴더 안쪽의 index.js 다음과 같이 수정

```js
import React from 'react';
import ReactDOM from 'react-dom';
import App from './App';
import { HashRouter } from 'react-router-dom';

ReactDOM.render(
	<React.StrictMode>
		<HashRouter>
			<App />
		</HashRouter>
	</React.StrictMode>,
	document.getElementById('root')
);
```

src 폴더 안쪽의 App.js 다음과 같이 수정

```js
function App() {
	return (
		<div className='App'>
			<h1>React Template Complete</h1>
		</div>
	);
}

export default App;
```
