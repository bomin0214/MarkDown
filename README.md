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
1. '<pre><code></code></pre>'
<pre><code>
'<pre><code></code></pre>'
</code></pre>

2. (```)
   
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

5.수평선 <hr/>

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

[GOOGLE](https://google.com)

[NAVER](https://naver.com "링크 설명(title)을 작성하세요.")

[상대적 참조](../users/login)


7.강조
======

- 인라인
> ' 백틱 기호 사용

<code>\강조강조강조강조강조 인라인됨.</code>
<pre><code>
\인라인\
</code></pre>


- 문자 강조
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

- 코드 강조
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

8.이미지
===
'''
![대체텍스트](이미지주소)
![대체텍스트](이미지주소 "설명")
![대체텍스트][참조]

[참조]: 이미지주소
[참조]: 이미지주소 "설명"
'''
![대체 텍스트(Alternative Text)](https://picsum.photos/1000/400 "링크 설명(Title)")
![이미지입니다!][Image]

[Image]: https://picsum.photos/500/300 "이미지입니다!"

- 사이즈 조절


'''
<img src="/path/to/img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="/path/to/img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
'''

- 이미지에 링크 추가

'''
[![HEROPY.DEV](/favicon.png)](https://heropy.dev/)
'''
[![HEROPY.DEV](/favicon.png)](https://heropy.dev/)

9.줄바꿈
===
- 3칸 이상 띄어쓰기를 하면 줄이 바뀐다.

10.표
==
- ㅇ
- ㅇ
- ㅇ

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

값 | 의미 | 기본값
---|:---:|---:
`static` | 유형(기준) 없음 / 배치 불가능 | `static`
`relative` | 요소 자신을 기준으로 배치 |
`absolute` | 위치 상 부모_(조상)요소를 기준으로 배치 |
`fixed` | 브라우저 창을 기준으로 배치 |
`sticky` | 스크롤 영역 기준으로 배치 |
</code></pre>
| 값 | 의미 | 기본값 |
|---|:---:|---:|
| `static` | 유형(기준) 없음 / 배치 불가능 | `static` |
| `relative` | 요소 자신을 기준으로 배치 |  |
| `absolute` | 위치 상 부모(조상)요소를 기준으로 배치 |  |
| `fixed` | 브라우저 창을 기준으로 배치 |  |
| `sticky` | 스크롤 영역 기준으로 배치 |  |

값 | 의미 | 기본값
---|:---:|---:
`static` | 유형(기준) 없음 / 배치 불가능 | `static`
`relative` | 요소 자신을 기준으로 배치 |
`absolute` | 위치 상 부모_(조상)요소를 기준으로 배치 |
`fixed` | 브라우저 창을 기준으로 배치 |
`sticky` | 스크롤 영역 기준으로 배치 |
