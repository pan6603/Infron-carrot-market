## Grid (레이아웃) - 2차원 레이아웃
> "Grid (레이아웃) - 2차원 레이아웃"은 웹 개발이나 앱 UI 디자인 등에서 **가로(행, row)**와 세로(열, column) 방향으로 구성된 격자 형태의 레이아웃을 말한다. 즉, 콘텐츠를 행과 열의 조합으로 배치하는 레이아웃 방식이다.

### Grid 레이아웃의 특징
+ 2차원 배치 가능
+ 레이아웃을 직관적으로 설계
+ 간격 조절이 편리함
+ 반응형 웹에 유리
+ 정렬 및 위치 지정이 자유로움
+ 코드가 깔끔함

index.html
```
    <div class="container">
        <header>MCOCL 블로그</header>
        <article>
            <h1>#1 HTML / CSS 공부하기</h1>
            <p>
                Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book
            </p>
            <p>
                It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
            </p>
        </article>
        <aside>
            <h2>menu</h2>
            <div>
                <div>menu1</div>
                <div>menu2</div>
                <div>menu3</div>
                <div>menu4</div>
            </div>
        </aside>
        <footer>
            MCOCL 블로그 footer
        </footer>
    </div>
```

style.css
```
body {
    width: 90%;
    max-width: 960px;
    margin: 2em auto;
    font: 0.9em/1.2 Arial, Helvetica, sans-serif;
}
.container {
    display: grid;
    grid-template-columns: 1fr 3fr;
    gap: 20px;
    /* 2) Grid 레이아웃 실습 */
    /* grid-template-areas: 
        "header header"
        "sidebar content"
        "footer footer"
    ; */
}
header,
footer {
    border-radius: 5px;
    padding: 10px;
    background-color: rgb(207, 232, 220);
    border: 2px solid rgb(79, 185, 227);
}
aside {
    border-right: 1px solid #999;
}

/* 1) Grid 레이아웃 실습 */
header {
    grid-column: 1 / 3;
    grid-row: 1;
}
aside {
    grid-column: 1;
    grid-row: 2 / 4;
}
article {
    grid-column: 2;
    grid-row: 2;
}
footer {
    grid-column: 2 / 3;
    grid-row: 3;
}

/* 2) Grid 레이아웃 실습 */
/* header {
    grid-area: header;
}
aside {
    grid-area: sidebar;
}
article {
    grid-area: content;
}
footer {
    grid-area: footer;
} */
```

### 쉽게 말하면?
표(table)처럼 콘텐츠를 가로, 세로로 정렬하는 방식

### 메모 정리
+ 
