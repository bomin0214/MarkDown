<pre><code>{}</code></pre>

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
<pre><code>{
This is an H1
=============
}</code></pre>

- 작은 제목

This is an H2
-------------
<pre><code>{
This is an H2
-------------
}</code></pre>

2.BlockQuote(인용)
   ====
">" 사용
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
<pre><code>{
  > This is a first blockqute.
  >	> This is a second blockqute.
  >	>	> This is a third blockqute.
}</code></pre>
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
> > > - 이 안에 다른 마크다운 요소 포함 가능

3.목록
   ====
- 순서 있는 목록(번호)
<pre><code>{
1. 첫번째
2. 두번째
3. 세번째
}</code></pre>
1. 첫번째
2. 두번째
3. 세번째
- 순서 없는 목록(*,+,-)
<pre><code>{
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑
}</code></pre>
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
<pre><code>{
This is a normal paragraph:

    This is a code block.
    
end code block.
}</code></pre>

This is a normal paragraph:

    This is a code block.
    
end code block.


> 한 줄 띄어쓰지 않으면 인식이 제대로 안되는 문제
<pre><code>{
This is a normal paragraph:
    This is a code block.
end code block.
}</code></pre>
This is a normal paragraph:
    This is a code block.
end code block.

- 코드 블럭 사용하는 방법
  ----
1. <pre><code>{}</code></pre>
<pre><code>{
<pre><code>{}</code></pre>
}</code></pre>

2. (```)
   
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

5.수평선 <hr/>
   ===
'''
* * *

***

*****

- - -

---------------------------------------
'''

6.링크
   =====
- 참조 링크
'''
[link keyword][id]

[id]: URL "Optional Title here"

// code
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"
'''
- Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"

- 외부링크
'''
사용문법: [Title](link)
적용예: [Google](https://google.com, "google link")
'''
- [Google](https://google.com, "google link")
- 자동 연결
'''
일반적인 URL 혹은 이메일주소인 경우 적절한 형식으로 링크를 형성한다.

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>
'''
* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>

7.강조
======
'''
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
'''
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
> 문장 중간에 사용할 경우에는 띄어쓰기를 사용하는 것이 좋다.

8.이미지
===
'''
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")
'''
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")

- 사이즈 조절
'''
<img src="/path/to/img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="/path/to/img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
'''

9.줄바꿈
===
- 3칸 이상 띄어쓰기를 하면 줄이 바뀐다.
