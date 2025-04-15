## overflow
> CSS에서 overflow는 요소(content)의 크기가 그 요소의 컨테이너 박스보다 클 때, 넘치는 부분을 어떻게 처리할지를 지정하는 속성이다.


### 실습코드
index.html
```
<div class="box">This box has a height and a width. This means that if there is too much content to be displayed within the assigned height, there will be an overflow situation. If overflow is set to hidden then any overflow will not be visible.</div>
```

stayle.css 
```
.box {
    border: 1px solid #333333;
    width: 200px;
    height: 100px;
    overflow: auto;
    /* overflow-y: scroll; */
}
```

### overflow 속성의 주요 값들
+ visible	기본값. 넘친 내용이 잘리지 않고 그냥 그대로 보임.
+ hidden	넘친 내용이 잘려서 안 보임. 스크롤바도 없음.
+ scroll	넘친 여부와 상관없이 항상 스크롤바가 생김.
+ auto	내용이 넘칠 때만 자동으로 스크롤바가 생김.


### 메모 정리
+ 콘텐츠 box안에 내용이 넘칠 경우 -> overflow: hidden 또는 scroll 사용하기
