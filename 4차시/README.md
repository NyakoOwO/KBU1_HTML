# 화면구현 4주차
#### 복습
---

```html
<form action="./hi.html">
    <label>이름<input type="text"></label><br>
    <label>비밀번호<input type="password"></label><br>
    <label>남자<input type="radio" name="gender" checked></label><br>
    <label>여자<input type="radio" name="gender" disabled></label><br>
    <input type="submit" value="클릭"><input type="reset">
</form>
```
으로할경우 링크에 해당 데이터가 유츌됨으로 그것을 막기위해
method="post"를 사용하여 숨길수있다

checked 를 할경우 체크를 할수있으며
disabled 는 체크를 비활성화한다


reset은 form에있는 값들을 초기값으로 바꾸는 버튼이다
```html
<input type="reset">
```


---


select는 리스트형식으로 option을 사용하여 리스트를 만들수있다
```html
<form action="#">
    <label>지역선택
        <select name="address">
            <option>서울시</option>
            <option>경기도</option>
            <option>전라도</option>
            <option>경상도</option>
        </select>
        <input type="submit" value="제출">
    </label>
</form>
```

option같은경우 value값을 지정하여도되나 없을시 option안에있는 내용으로 
address=서울# 이라고 주소창에 뜨게된다

---

게시판같은곳에서 주로 사용이 된다
cols, rows 는 기본크기의 값을 지정한다
placeholder 는 입력이없을때 뜨는내용을 적는다
```html
<form action="#">
    <textarea name="memo" id="" cols="30" rows="10"></textarea>
</form>
```

---
Css
---
### Css적용 순서
##### 인라인 스타일 시트 > 내부 스타일 시트 > 외부 스타일 시트
<br>
내부 스타일 시트
```html
<!-- Html 파일 (index.html) -->
<style>
    /*Css의 주석*/
    h1{
        color: red;
    }
</style>
```
<br>
외부 스타일 시트
```html
<!-- Html 파일 (index.html) -->
<head>
    <link rel="stylesheet" herf="index.css">
</head>
<h1>Hello World</h1>
```
```css
/* Css 파일(index.css) */
h1{
    color:blue;
}
```
<br>
```html
<!-- Html 파일 (index.html) -->
<style>
    @import url("index.css")
</style>
```
<br>
```html
<!-- Html 파일 (index.html) -->
<style>
    @import "index.css"
</style>
```
<br>
인라인 스타일 시트
```html
<!-- Html 파일 (index.html) -->
<h1 style="color=green;">
```


---
Css 속성
---
```html
<!--[ id는 1개만 사용이가능하다 ]-->
<h1 id="title">
    Css 배우기
</h1>
<!--[ class는 여러개를 사용이가능하다 ]-->
<h1 class="title">
    Css 배우기
</h1>
```


```css
/* [ * = 모든 속성 ] */
*{
    color: Red;         /* 글시 색상을 Red로 설정 */
}


/* [ h1 = 모든 h1 속성 ] */
hr{
    border: 1px solid green; /* 테두리를 초록색 1px 테두리를 만들기*/
}

/* [ #title = id값이 title인 속성 ] */
#title{
    font-size: 15px;    /* 폰트크기를 15px로 설정 */
    background: yellow; /* 배경색상을 노랑색으로설정 */
}

/* [ .title = class값이 title인 속성 ] */
.title{
    color:blue;
}


```