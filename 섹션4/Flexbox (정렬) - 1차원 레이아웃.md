## Flexbox (정렬) - 1차원 레이아웃
> Flexbox(플렉스박스)는 CSS의 1차원 레이아웃 시스템으로, 요소들을 가로 또는 세로 방향 중 한 방향(축 하나)으로 정렬하고 배치할 수 있도록 도와준다.

### "1차원 레이아웃"이란?
한 방향(가로 또는 세로)으로만 정렬을 제어할 수 있다는 뜻이다.
예: 가로 정렬 (row) 또는 세로 정렬 (column) 중 하나만 선택해서 사용할 수 있음.

index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="./styles.css">
    <title>Document</title>
</head>
<body>
    <div>
        <button>Smile</button>
        <button>Laugh</button>
        <button>Wink</button>
        <button>Shrug</button>
        <button>Blush</button>
    </div>
</body>
</html>
```

style.css
```
html {
  font-family: sans-serif;
}
div {
  width: 70%;
  margin: 100px auto;
  height: 350px;
  border: 1px solid black;

  /* flex 실습 */
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 15px;
  /* flex-direction: column; */
}
button {
  /* flex: 1; */
  width: 100px;
}
button:nth-of-type(2) {
  align-self: flex-end;
  /* flex: 1; */
}
```


### 메모 정리 
+ justify-content 통해서 가로 정렬 시킬 수 있다.
+ align-items 통해서 세로 방향 정렬 시킬 수 있다.
+ flex-direction 사용하면 세로 방향으로 정렬 시킬 수 있다. 
