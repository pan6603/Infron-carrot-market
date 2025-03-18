## a태그는 무엇인가? 
> a태그는 HTML에서 주로 다른 페이지로 이동하는 하이퍼링크를 생성할 때 사용한다.

### 사용이유 
a 태그는 웹에서 링크(하이퍼링크)를 만들기 위해 필수적인 요소이다. 웹의 기본 개념이 페이지 간 이동이므로, <a> 태그가 없다면 웹사이트 간 연결이 어려워진다.

### 웹페이지 간 이동이 쉬움
+ href 속성만 설정하면 간단하게 다른 페이지로 연결 가능
+ 네비게이션 메뉴, 외부 링크, 다운로드 등에 필수

### 실습 코드 

3_text.html 
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <p>
        I'm creating a link to 
        <a href="https://www.mozilla.org/en-US" title="The best place to find more">the Mozilla homepage</a>
    </p>
    <a href="https://www.mozilla.org/en-US/">
        <img src="./images/test_img.png" alt="Mozilla homepage" style="height: 200px; width: 200px;"/>
    </a>
    <p>
        This is the index file
        <a href="index.html">Link</a>
    </p>
</body>
</html>
```

### 메모 정리 
+ 클릭 한 번으로 원하는 페이지나 정보로 쉽게 이동 가능하다.
+ 네비게이션, 버튼 스타일링 등을 통해 직관적인 사용자 경험을 제공 할 수 있다. 







