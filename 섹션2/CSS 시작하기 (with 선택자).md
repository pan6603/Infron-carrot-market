## CSS는 무엇인가?
> CSS는 HTML 요소의 스타일을 지정하는 언어이다.
즉, HTML이 웹 페이지의 구조를 담당한다면, CSS는 디자인과 레이아웃을 담당을 하다.

### CSS의 역할
+ 글자 색상, 크기, 글꼴 변경
+ 배경색, 배경 이미지 설정
+ 레이아웃 조정 (박스 크기, 정렬, 여백 등)
+ 반응형 디자인 (모바일, 태블릿, 데스크톱)
+ 애니메이션 및 효과 추가

### 왜 사용하는가? 
CSS는 HTML 요소의 스타일을 지정하여 웹페이지를 더욱 아름답고 사용하기 쉽게 만들기 위해 사용된다.
HTML은 기본적으로 구조만 정의할 수 있고, 디자인 기능이 부족하기 때문에 CSS가 필수이다.

### 실습 코드 

index.html 
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="./styles.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>레벨 1 제목입니다</h1>

    <p>이것은 단락입니다. 본문에는 <span>span 요소</span>와 <a href="http://example.com">링크</a>가 있습니다.</p>

    <p>이것은 두 번째 단락입니다. <em>강조된</em> 요소를 포함합니다.</p>

    <ul>
        <li id="myidname">항목 하나</li>
        <li class="special">항목 둘</li>
        <li class="special">항목 <em>셋</em></li>
    </ul>

    <h1>I am a level one heading</h1>
    <div class="test">
        <p>
            <span>
                Hi test span
            </span>
        </p>
    </div>

    <p>This is a paragraph of text. In the text is a <span>span element</span> 
    and also a <a href="http://example.com">link</a>.</p>

    <p>This is the second paragraph. It contains an <em>emphasized</em> element.</p>

    <ul>
        <li>Item one</li>
        <li>Item two</li>
        <li>Item <em>three</em></li>
    </ul>
</body>
</html>
```

styles.css
```
h1 {
    color: red;
}

p, li {
    color: green;
}

li {
    list-style-type: none;
}

.special {
    color: orange;
    font-weight: bold;
}

.test span {
    font-size: 50px;
}

li.special {
    font-weight: bold;
}
```



### 메모정리 
+ 개발자 도구 F12에서 테스트로 색상 추가, 변경이 가능하다.
+ , 콤마를 이용하여 한번에 지정자를 변경할 수 있다.
+ CSS 선택자만 잘해도 CSS 작성이 수월해질 수 있다.
