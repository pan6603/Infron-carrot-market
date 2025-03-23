## CSS의 상속과 우선순위
> CSS 상속은 부모 요소의 스타일이 자식 요소에게 자동으로 전달되는 것이다. 우선순위는 여러 스타일이 충돌할 때 어떤 스타일이 이길지 결정하는 규칙이다.


### 실습 코드
3_priority.html
```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>나의 CSS 실험</title>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
      <div id="outer" class="container">
          <div id="inner" class="container">
              <ul>
                  <li class="nav"><a href="#">One</a></li>
                  <li class="nav"><a href="#">Two</a></li>
              </ul>
          </div>
      </div>                            
</body>
</html>

```

styles.css
```
/* 1. specificity: 1-0-1 */
#outer a {
    background-color: red;
}
        
/* 2. specificity: 2-0-1 */
#outer #inner a {
    background-color: blue;
}

/* 3. specificity: 1-0-4 */
#outer div ul li a {
    color: yellow;
}

/* 4. specificity: 1-1-3 */
#outer div ul .nav a {
    color: white;
}

/* 5. specificity: 0-2-4 */
div div li:nth-child(2) a:hover {
    border: 10px solid green;
}

/* 6. specificity: 0-2-3 */
div li:nth-child(2) a:hover {
    border: 10px dashed red;
}

/* 7. specificity: 0-3-3 */
/* div div .nav:nth-child(2) a:hover {
    border: 10px double yellow;
} */

a {
    display: inline-block;
    line-height: 40px;
    font-size: 20px;
    text-decoration: none;
    text-align: center;
    width: 200px;
    margin-bottom: 10px;
}

ul {
    padding: 0;
}

li {
    list-style-type: none;
}            
    
```

### 메모 정리 
+ 태그안에 style 속성 사용하지 않기
+ !important 사용하면 제일 1순위로 선택자 지정이 됨.
