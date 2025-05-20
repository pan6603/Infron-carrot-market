## Grid (기본) - 2차원 레이아웃
> "Grid (기본) - 2차원 레이아웃"은 웹 프론트엔드 개발에서 CSS Grid Layout을 의미하며, 2차원적인 레이아웃을 만들 수 있도록 도와주는 CSS의 레이아웃 시스템이다.

### 핵심 특징
+ 2차원 레이아웃	행(row)과 열(column)을 동시에 다룰 수 있음 (예: flex는 1차원만 가능)
+ 반응형 웹 제작 용이	다양한 해상도에 맞게 정렬 가능
+ 간단한 문법	코드만으로 복잡한 배치 구현 가능
+ 정렬이 자유로움	칸 병합, 공간 분할 등이 쉬움


index.html
```
    <div class="container">
        <div>1-One</div>
        <div>2-Twe</div>
        <div>3-Three</div>
        <div>4-Four</div>
        <div>5-Five</div>
        <div>6-Six</div>
        <div>7-Seven</div>
        <div>8-Eight</div>
    </div>
```


style.css
```
.container {
    width: 70%;
    margin: 100px auto;
    padding: 10px;
    background-color: #FEFCF3;
    border: 2px solid #2B3A55;

    /* Grid 실습 */
    display: grid;
    /* grid-template-columns: repeat(3, 100px); */
    grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
    /* grid-template-rows: 100px; */
    grid-auto-rows: minmax(100px, auto);
    gap: 10px;
}

.container > div {
    background-color: #FFE15D;
}
```


### 메모 정리 
+ grid-template-columns 속성을 사용하면 열 넓이 크기 지정.
+ grid-template-rows 속성을 사용하면 행 넓이 크기 지정.
+ grid-auto-rows 속성을 사용시 전체 행 넓이 똑같이 지정.
+ 1fr을 사용하면 부모 컨테이너 안에서 차지할 수 있는 비율.  
