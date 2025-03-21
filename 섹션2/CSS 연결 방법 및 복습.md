## CSS 연결 방법 및 복습
> CSS 연결이란 웹페이지에서 HTML 파일과 CSS 파일을 연결하여 스타일을 적용하는 것을 말한다. <br> 쉽게 말해, HTML로는 웹페이지의 구조(뼈대)를 만들고, CSS는 그 구조에 디자인(색상, 폰트, 배치 등)을 입히는 역할을 한다.

### 왜 사용하는가? 
CSS를 사용해서 디자인과 레이아웃을 조정하기 때문에 사용. 

### 1. 외부 CSS 연결 (가장 많이 사용됨)
HTML 파일 안에서 외부에 저장된 CSS 파일을 링크해서 사용하는 방식입니다.

```
<head>
  <link rel="stylesheet" href="style.css">
</head>

```

### 2. 내부 CSS (Internal)
HTML 파일 안에 <style> 태그를 사용해서 직접 CSS를 작성하는 방식이에요.

```
<head>
  <style>
    body {
      background-color: lightblue;
    }
  </style>
</head>

```

### 3. 인라인 CSS (Inline)
HTML 태그 안에 직접 style 속성을 이용해서 스타일을 적용하는 방식이에요.

```
<p style="color: red;">안녕하세요!</p>
```

### 실습 코드

2_index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./styles.css">
    <title>Document</title>
</head>
<body>
    <h1>헬로우 월드!</h1>
    <p>이것은 나의 첫 번째 CSS 예제입니다</p>
    <div class="box">
        <p class="special">p1</p>
        <p>p2</p>
        <p>p3</p>
    </div>
    <div>
        <p>
            ppppp
        </p>
    </div>    
</body>
</html>
```

style.css 

```
h1 {
    color: blue;
    background-color: yellow;
    border: 1px solid black;
}

.special {
    color: red;
}   
```


### 메모 정리 
+ 태그 안에 style 적용하지 않기 이유는 나중에 유지보수가 힘들어짐.
+ 문단 태그 안에 div요소 넣으면 style 적용되지 않는다. 
