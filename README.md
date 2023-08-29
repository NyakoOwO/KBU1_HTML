# 화면구현 1차시


HTML태그 <텍스트 태그>   
&quot; = `&quot;`   
&apos; = `&apos;`   
&lt; = `&lt;`   
&gt; = `&gt;`   
&amp; = `&amp;`   

공백 = `&nbsp;`   

strong = 굵게   
b = 굵게   
i = 기울이기   
em = 약간 기울이기   
del = 그은선   
ins = 밑줄   
sup = 위에를 기준   
sub = 아래를 기준   
mark = 하이라이팅 표시   

<! -- --> = 주석처리   
./ 현재 파일과 같은 폴더위치
../ 현재 파일의 상위 폴더위치

h1 ~ h6 = 글자 크기 태그    
br = 줄바꿈 태그   
hr = 구분선 태그   

a = 하이퍼 링크   
  └ href="이동할 링크"   


----
`아래의 내용처럼 출력하시오`

![image](https://github.com/Bluebla1004/Screen_implementation-2/assets/73012354/d697b94b-17dd-4b3b-9290-cabbc8be4859)

```html
안녕하세요<br>
저의 이름은&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;홍길동&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;입니다.
```


----
`아래의 내용처럼 출력하시오`

![image](https://github.com/Bluebla1004/Screen_implementation-2/assets/73012354/c51ddc56-b80f-4165-8cac-2e854b7188f4)

```html
<hr>
<h1>
    아래의 정답은 무엇일까요??
</h1>
<hr>
<h4>
    아래의 문제는 &quot;&lt;pre&gt;&quot;를 사용하지 마세요
</h4>
<hr>
<p>
    10 &divide; 5 = (&nbsp;&nbsp;&nbsp;)
</p>
<p>
    10 * 5 = (&nbsp;&nbsp;&nbsp;)
</p>
```


----
`아래의 내용처럼 출력하시오`

![image](https://github.com/Bluebla1004/Screen_implementation-2/assets/73012354/176b8e91-1d9a-48b2-b860-710121790ac3)

```html
<p>
    <mark>
        HTML
    </mark>
</p>
<p>
    <I>
        JAVA
    </I>
</p>
<p>
    <B>
        PYTHON
    </B>
</p>
```


----
`웹페이지, 로컬파일 이동하는코드를 만드시오`

```html
# <a href="링크">표시할 글시</a>

<a href="https://naver.com">네이버로</a>
<a href="./page.html">페이지로</a>
# 현재 메인파일에 page.html이없을경우 흰백지가나온다
```
