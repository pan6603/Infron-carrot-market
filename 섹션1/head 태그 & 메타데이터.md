## head 태그 & 메타데이터
+ head 태그는 HTML 문서의 메타데이터(문서의 정보)를 포함하는 부분이다. 브라우저에는 직접 표시되지 않지만, 웹페이지의 동작과 스타일을 설정할 수 있다.

### 실습 코드 

index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta
        name="description"
        content="The MDN Web Docs Learning Area aims to provide
        complete beginners to the Web with all they need to know to get
        started with developing web sites and applications."
    />
    <link rel="stylesheet" href="my-css-file.css" />
    <script src="my-js-file.js" defer></script>

    <title>Document</title>
</head>
<body>
    <h1>Hello World</h1>
    <p>My cat is cute</p>
    <p>My cat is cute</p>

    <span>span is inline</span><span>span is inline</span><span>span is inline</span>
</body>
</html>
```
+ CSS 외부 파일을 연결하기 link태그 사용
+ js 외부 파일을 연결하기 script 태그 사용 

my-css-file.css 
```
body {
    background-color: yellow;
}
```
+ body 태그 배경화면을 yellow 설정

my-js-file.js 
```
console.log("Hello Js");
```
+ js파일 잘 연결이 되었는지 확인하기 위해 크롬 F12 단축키 통해서 console.log 확인하기 




### 📌 메모 정리
+ head 태그는 화면에 보이지 않음.
+ viewport는 디바이스 화면에 어떻게 보일 지 비율 맞추는 태그
+ meta name="description" 검색 결과에 표시될 페이지 설명 제공
+ 외부 CSS 파일을 연결시키기 위해 link 태그 사용
+ 외부 Js 파일을 연결시키기 위해 Script 태그 사용 
