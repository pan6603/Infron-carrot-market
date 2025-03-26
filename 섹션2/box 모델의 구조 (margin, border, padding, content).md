### box 모델의 구조 (margin, border, padding, content)

+ 박스 모델은 Content → Padding → Border → Margin 순서로 구성
+ 기본적으로 width와 height는 content 크기만 포함
+ box-sizing: border-box;을 사용하면 전체 크기를 고정할 수 있어 유용함!


4_box_model.html

```
 <div class="box">box1</div>
 <div class="box">box2</div>
```

5-1_box_model.css

```
.box {
    width: 350px;
    height: 150px;
    margin: 20px;
    padding: 10px;
    border: 5px solid black;
    box-sizing: border-box;
}

```



### 메모 정리 
+ div와 span은 content 안에 들어간다.
+ box 구조는 margin, border, padding, content이다.
+ 태그와 class 속성을 한번에 만드는 방법은 -> div.box 입력하기
+ 태그를 한번에 여러개 만드는 방법 -> div * 5 입력하기
+ F12 개발자 도구 박스 모델에서 margin, border, padding, content 등 값을 넣어 실험해보기
   
    
