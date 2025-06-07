## position 이란? 
> CSS에서 position은 HTML 요소가 문서 안에서 어떻게 배치될지를 결정하는 속성이다. position 속성은 레이아웃을 만들거나 특정 요소의 위치를 조정할 때 아주 중요한 역할을 한다.

### 사용 이유
CSS에서 position 속성을 사용하는 이유는 웹 페이지의 요소를 원하는 위치에 정확하게 배치하거나, 동적으로 움직이게 만들기 위해서이다.



#### position.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="21_position.css">
    <title>Document</title>
</head>
<body>
    <div class="box">
        <div class="box1">static</div>
        <div class="box2">relative</div>
        <div class="box3">absolute1</div>
        <div class="box3_2">absolute2</div>
        <div class="box4">sticky</div>
        <div class="box5">fixed</div>
    </div>
</body>
</html>
```

#### position.css
```
.box {
    position: relative;
    width: 900px;
    height: 200vh;
    margin: 0 auto;
    border: 2px solid red;
    background-color: blanchedalmond;
}
.box1, .box2, .box3, .box4, .box5, .box3_2 {
    width: 70px;
    height: 70px;
}
.box1 {
    background-color: red;
    /* 기준 X */
    position: static;
    left: 30px;
    /* right: ;
    top: ;
    bottom: ; */
}
.box2 {
    background-color: orange;
    /* 내가 기준(박스는 움직이지만 기존 공간은 차지) */
    position: relative;
    /* left: 30px; */
    /* bottom: 30px; */
    /* right: 30px; */
    /* top: 120vh; */
}
.box3 {
    background-color: yellow;
    /* 위치 상(컨테이닝 블록) 부모가 기준 */
    position: absolute;
    left: 50px;
    top: 0;
    z-index: 50;
}
.box3_2 {
    background-color: violet;
    position: absolute;
    left: 100px;
    top: 0;
    z-index: 30;
}
.box4 {
    background-color: green;
    /* 스크롤이 기준 */
    position: sticky;
    top: 70px;
    left: 70px;
}
.box5 {
    background-color: blue;
    /* 브라우저가 기준 */
    position: fixed;
}
```


### 메모 정리 
+ 부모는 position: relative이고, 자식은 position: absolute; 이다.
+ sticky 많이 사용하지 않음.
+ position: fixed는 팝업을 만들때 많이 사용한다. 
