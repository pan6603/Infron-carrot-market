## Floats - 신문같은 레이아웃
> CSS의 float 속성은 원래 이미지를 텍스트 옆에 배치하려고 만든 기능이다.

floats.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="20_floats.css">
    <title>Document</title>
</head>
<body>
    <h1>Simple float 예제</h1>

    <div class="wrapper">
        <div class="box">float</div>
        <p class="special">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla luctus aliquam dolor, eu lacinia lorem placerat vulputate. Duis felis orci, pulvinar id metus ut, rutrum luctus orci. Cras porttitor imperdiet nunc, at ultricies tellus laoreet sit amet. </p>
    </div>
    <p class="cleand">Sed auctor cursus massa at porta. Integer ligula ipsum, tristique sit amet orci vel, viverra egestas ligula. Curabitur vehicula tellus neque, ac ornare ex malesuada et. In vitae convallis lacus. Aliquam erat volutpat. Suspendisse ac imperdiet turpis. Aenean finibus sollicitudin eros pharetra congue. Duis ornare egestas augue ut luctus. Proin blandit quam nec lacus varius commodo et a urna. Ut id ornare felis, eget fermentum sapien.</p>
    <p>Nam vulputate diam nec tempor bibendum. Donec luctus augue eget malesuada ultrices. Phasellus turpis est, posuere sit amet dapibus ut, facilisis sed est. Nam id risus quis ante semper consectetur eget aliquam lorem. Vivamus tristique elit dolor, sed pretium metus suscipit vel. Mauris ultricies lectus sed lobortis finibus. Vivamus eu urna eget velit cursus viverra quis vestibulum sem. Aliquam tincidunt eget purus in interdum. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</p>
</body>
</html>
```

floats.css
```
body {
    width: 90%;
    max-width: 900px;
    margin: 0 auto;
    font: .9em/1.2 Arial, Helvetica, sans-serif
}
.box {
    float: left;
    margin: 10px;
    width: 150px;
    height: 100px;
    border-radius: 5px;
    background-color: #FCF9BE;
    padding: 1em;
}
.special {
    background-color: yellowgreen;
    padding: 10px;
    color: #fff;
}
.cleand {
    clear: left;
}
.wrapper {
    background-color: violet;
    padding: 10px;
    /* overflow: auto; */
    display: flow-root;
}
```

### 📝 요약
+ Float은 요소를 좌우로 띄워서 배치함
+ 신문 같은 레이아웃은 이미지와 텍스트, 광고 등이 칼럼처럼 나뉜 형태
+ 예전에는 float으로 구현했지만, 지금은 Flexbox나 Grid를 권장





### 메모 정리
