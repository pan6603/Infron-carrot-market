## CSS 의 단위는 무엇인가?
> CSS에서 단위(unit)는 길이, 크기, 간격 등을 지정할 때 숫자와 함께 사용하는 기준이다.

index.html
```
<div class="wrapper">
   <div class="box px">px, Hello Html</div>
   <div class="box vw">vw, Hello html</div>
   <div class="box em">em, Hello html</div>
   <div class="box rem">rem, Hello html</div>
   <div class="p_box"></div>
</div>
```

stayle.css
```
.wrapper {
    font-size: 30px;
}
.box {
    width: 500px;
    height: 100px;
    border: 2px solid red;
}
.px {
    font-size: 16px;
}
.vw {
    font-size: 3vw;
}
.em {
    font-size: 50%;
}
.rem {
    font-size: 1rem;
}
.p_box {
    height: 100px;
    width: 50%;
    border: 2px solid blue;
}
```


## 메모 정리
+ px은 화면의 구성 요소의 가장 작은 단위다.
+ 기본 html의 폰트 사이즈는 16px이다. 



