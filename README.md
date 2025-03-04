1.Headers 헤더
   ==============

# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6

<pre><code>{
# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6
}</code></pre> 

- 큰 제목

This is an H1
=============
<pre><code>
This is an H1
=============
</code></pre>

- 작은 제목

This is an H2
-------------
<pre><code>
This is an H2
-------------
</code></pre>

2.BlockQuote(인용)
   ====
">" 사용
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
<pre><code>
  > This is a first blockqute.
  >	> This is a second blockqute.
  >	>	> This is a third blockqute.
</code></pre>
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
> > > - 이 안에 다른 마크다운 요소 포함 가능

3.목록
   ====
- 순서 있는 목록(번호)
<pre><code>
1. 첫번째
2. 두번째
3. 세번째
</code></pre>
1. 첫번째
2. 두번째
3. 세번째
- 순서 없는 목록(*,+,-)
<pre><code>
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑
</code></pre>
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑

4.코드
   ====
- 들여쓰기
4개의 공백 또는 하나의 탭으로 들여쓰기를 만나면 변환되기 시작하여 들여쓰지 않은 행을 만날때까지 변환이 계속된다.
<pre><code>
This is a normal paragraph:

    This is a code block.
    
end code block.
</code></pre>


> 결과
***
This is a normal paragraph:

    This is a code block.
    
end code block.


> 한 줄 띄어쓰지 않으면 인식이 제대로 안되는 문제
<pre><code>
This is a normal paragraph:
    This is a code block.
end code block.
</code></pre>
This is a normal paragraph:
    This is a code block.
end code block.

- 코드 블럭 사용하는 방법
  ----
1. `<pre><code></code></pre>`
2. (```)
   
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

5.수평선 <hr/>
==

<pre><code>
* * *

***

*****

- - -

---------------------------------------
</code></pre>

* * *

***

*****

- - -

---------------------------------------

6.링크
   =====

<pre><code>
[이름](링크)
[이름](링크 "설명")
[이름][참조]
</code></pre>
<pre><code>
[GOOGLE](https://google.com)

[NAVER](https://naver.com "링크 설명(title)을 작성하세요.")

[상대적 참조](../users/login)
</code></pre>
[GOOGLE](https://google.com)

[NAVER](https://naver.com "링크 설명(title)을 작성하세요.")

[상대적 참조](../users/login)


7.강조
======
인라인
-------
`<code>인라인 코드 이렇게 작성함.</code>`

코드 안에 코드 보이게 하는법
---
백택 (`) 이용하기

문자 강조
   ---
<pre><code>
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
</code></pre>
*single asterisks*   
_single underscores_   
**double asterisks**   
__double underscores__   
~~cancelline~~   
> 문장 중간에 사용할 경우에는 띄어쓰기를 사용하는 것이 좋다.

코드 강조
  ---
<pre><code>
```html
<a href="https://www.google.co.kr/" target="_blank">GOOGLE</a>
```

```css
.list > li {
  position: absolute;
  top: 40px;
}
```

```javascript
function add(a, b = 1) {
  console.log(a, b)
  return a + b
}
```

```bash
$ npm run dev
```
 
```python
s = "Python syntax highlighting"
print s
```
 
```plaintext
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```
</code></pre>
```html
<a href="https://www.google.co.kr/" target="_blank">GOOGLE</a>
```

```css
.list > li {
  position: absolute;
  top: 40px;
}
```

```javascript
function add(a, b = 1) {
  console.log(a, b)
  return a + b
}
```

```bash
$ npm run dev
```
 
```python
s = "Python syntax highlighting"
print s
```
 
```plaintext
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```
코드 안에 <> 넣는법
--
`&lt; 와 &gt;`

8.링크
===
<pre><code>
인라인 링크는 아래처럼
[인라인 링크](https://velog.io/)

url 링크는 아래처럼
&lt;https://velog.io/&gt;

참조 링크
[velog]:(https://velog.io/)
</code></pre>

9.이미지
   ==
<pre><code>
![이미지 설명](이미지 링크)
![고양이애옹](https://cdn.pixabay.com/photo/2019/03/13/08/29/cat-4052454_1280.jpg)
</code></pre>

![고양이애옹](https://cdn.pixabay.com/photo/2019/03/13/08/29/cat-4052454_1280.jpg)

이미지에 링크 걸기
  ---
<pre><code>
[![이미지 설명](이미지 링크)](연결하고자하는 url "마우스 오버 시 나타낼 링크 title")
[![고양이애옹](https://cdn.pixabay.com/photo/2019/03/13/08/29/cat-4052454_1280.jpg)](https://cdn.pixabay.com/photo/2019/03/13/08/29/cat-4052454_1280.jpg"이미지 무료 사이트 pixabay")
</code></pre>

[![고양이애옹](https://cdn.pixabay.com/photo/2019/03/13/08/29/cat-4052454_1280.jpg)](https://cdn.pixabay.com/photo/2019/03/13/08/29/cat-4052454_1280.jpg"이미지 무료 사이트 pixabay")

10.줄바꿈
===
- 3칸 이상 띄어쓰기를 하면 줄이 바뀐다.

11.표
==

- <code>---</code> , <code>:--- </code>: 좌측 정렬
- <code>:---:</code> : 가운데 정렬
- <code>---:</code> :우측 정렬

<pre><code>
| 헤더 | 헤더 | 헤더 |
|---|---|---|
| 셀 | 셀 | 셀 |
| 셀 | 셀 | 셀 |

헤더 | 헤더 | 헤더
---|---|---
셀 | 셀 | 셀
셀 | 셀 | 셀
</code></pre>
<pre><code>
| 값 | 의미 | 기본값 |
|---|:---:|---:|
| `static` | 유형(기준) 없음 / 배치 불가능 | `static` |
| `relative` | 요소 자신을 기준으로 배치 |  |
| `absolute` | 위치 상 부모(조상)요소를 기준으로 배치 |  |
| `fixed` | 브라우저 창을 기준으로 배치 |  |
| `sticky` | 스크롤 영역 기준으로 배치 |  |

</code></pre>
| 값 | 의미 | 기본값 |
|---|:---:|---:|
| `static` | 유형(기준) 없음 / 배치 불가능 | `static` |
| `relative` | 요소 자신을 기준으로 배치 |  |
| `absolute` | 위치 상 부모(조상)요소를 기준으로 배치 |  |
| `fixed` | 브라우저 창을 기준으로 배치 |  |
| `sticky` | 스크롤 영역 기준으로 배치 |  |

12.체크박스(Check Box)
===
x가 넣어지면 체크된 체크박스 생성
<pre><code>
- [ ] 운동 하기
- [x] 강의 듣기
</code></pre>
- [ ] 운동 하기
- [x] 강의 듣기

13.이모지
===
- window10: 윈도우 + .
- max: command + control + 스페이스바
