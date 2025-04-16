## form태그는 무엇인가?
> form 태그는 사용자로부터 입력을 받기 위한 HTML 태그이다. <br> 예를 들면 로그인 폼, 회원가입 폼, 검색창, 설문조사 등에서 사용된다.


### form 태그 실습 코드 

#### index.html
```
<!-- 3. form -->
    <form>
        <div>
            <label for="name">Name</label>
            <input type="text" id="name">
        </div>
        <div>
            <label for="email">Email</label>
            <input type="email" id="email">
        </div>
        
        <div class="buttons">
            <input type="submit" value="Submit">
        </div>
    </form>
```

#### style.css
```
/* 3. form */
form {
    width: 500px;
}
input[type="text"],
input[type="email"] {
  border: 2px solid #000;
  margin: 0 0 1em 0;
  padding: 10px;
  width: 100%;
}
input[type="submit"] {
  border: 3px solid #333;
  background-color: #999;
  border-radius: 5px;
  padding: 10px 2em;
  font-weight: bold;
  color: #fff;
}
input[type="submit"]:hover {
  background-color: #333;
}
```


### 메모 정리
+ form 사용자로부터 값을 입력을 받는 태그이다.
