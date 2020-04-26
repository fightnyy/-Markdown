

## 1.마크다운 사용법 

###### 	1 헤더

+ ###### 글머리: 1~6 까지 지원

```markdown
# This is h1
## this is h2
### this is h3 
#### this is h4
##### this is h5
###### this is h6

```

***



###### 2 Blockquote

* ###### 이메일에서 사용하는 '>' 블럭인용문자를 사용

```
> This is a first block quote

>> This is a second block quote
```

###### 사용예시

> This is a first block quote
>
> > This is a second block quote
> >
> > > This is a third block quote



이 안에서는 다른 마크다운 요소를 포함할 수 있다고 한다. 

> * 이런방식으로
>
>   ```
>   아니면 이런방식으로든
>   ```

<hr/> 



###### 3. 목록

+ ###### 순서있는 목록(번호)

  순서 있는 목록은 숫자와 번호를 사용한다.

  ```
  1. 안녕
  2. 반가워
  3. 나도 그래
  ```

  

###### 사용예시

1. 안녕
2. 반가워
3. 나도그래

여기서 재미있는 점은 숫자가 중요하다는 것이다.

```
1. 안녕
3. 나도 그래
2. 반가워
```

이렇게 해도 

1. 안녕

2. 반가워

3. 나도 그래 

   라고 출력된다.

***

* ###### 순서없는 목록(글머리 지원+,*,-) 

  ```
  * 빨강
  	+ 노랑
  		- 파랑
  
  이렇게도(혼합) 사용 할 수 있고
  
  *빨강
  	*노랑
  		*파랑
  이렇게도(혼합X) 사용 할 수 있다.
  ```

  

###### 사용예시

* 빨강
  + 노랑
    - 파랑

이렇게도(혼합) 사용할 수 있고

* 빨강
  * 노랑
    - 파랑

이렇게도(혼합x) 사용 할 수 있다. 

<hr/>



###### 4. 코드블록

-코드블록 방식에는 2가지를 이용 할 수 있다.

```
<pre>
	<code>
		{code}
	</code>
</pre>


or


​```
	{code}
​```
```



방식이다. 하지만 나는 typora를 사용하고 있는데 여기서는 그냥 option+command+c를 누르기만 하면 되어서 간편하다. 

###### 사용예시


```c
printf("Hello World!");
```

```c
printf("Good to see you")
```

<hr/>





###### 5.수평선

-이거는 느낌이 HTML과 비슷하다. hr/을 태그로 써주면된다. 또한 다양한 방법도 많다.

```
</hr>
***
______
_ _ _

```

###### 사용예시

<hr/>

_ _ _

____________

***



###### 6.링크

+ 참조링크

  ```
  [link keyword][id]
  [id]:url "선택적인 제목은 여기에 써줘요"
  
  //code
  Link: [Google][googlelink]
  [googlelink]: https://google.com "Go google"
  -----------------------------------------------------------------------
  [GOOGLE](https://google.com)
  
  [NAVER](https://naver.com "링크 설명(title)을 작성하세요.")
  
  [상대적 참조](../users/login)
  
  [Dribbble][Dribbble link]
  [Dribbble link]: https://dribbble.com
  
  [GitHub][1]
  [1]: https://github.com
  
  문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.
  
  다음과 같이 문서 내 일반 URL이나 꺾쇠 괄호(`< >`, Angle Brackets)안의 URL은 자동으로 링크를 사용합니다.
  구글 홈페이지: https://google.com
  네이버 홈페이지: <https://naver.com>
  
  
  
  [참조 링크]: https://naver.com "네이버로 이동합니다!"
  
  ```

  ###### 사용예시

  Link: [Google][googlelink]

  [googlelink]: https://google.com

  ######  [Google][https://google.com]

  [Naver](https://naver.com "Let's go to Naver")

  [상대적참조](../users/login)

  [Dribble](https://drrible.com)

  [Github][1]

  [1]: https://github.com

  문서 안에서 [참조링크]를 그대로 사용 할 수 도 있습니다.

  다음과 같이 문서 내 일반 URL이나 꺾쇠 괄호('< >',Angle Brackets)안의 URL은 자동으로 링크를 사용합니다. 

  구글 홈페이지: https://google.com

  네이버 홈페이지: <https://naver.com>

***



###### 7.강조

```
*word*
**word**
_word_
__word__
~~word~~
```



###### 사용예시

*word*

**word**

_word_

__word__

~~word~~

문자 중간에 사용하려면 띄어쓰기를 잘 해주는것이 좋다.

```
sentence blah blah *blah* blah
```

sentence blah blah *blah* blah

***

###### 8.이미지

`<img>`로 변환됩니다.
링크과 비슷하지만 앞에 `!`가 붙습니다.

```
![대체 텍스트(alternative text)를 입력하세요!](http://www.gstatic.com/webp/gallery/5.jpg "링크 설명(title)을 작성하세요.")

![Kayak][logo]

[logo]: http://www.gstatic.com/webp/gallery/2.jpg "To go kayaking."
```



![대체 텍스트를 입력하세요!](http://www.gstatic.com/webp/gallery/5.jpg "링크설명을 작성하자")

![kayak][logo]

[logo]: http://www.gstatic.com/webp/gallery/2.jpg "To go kayaking. "

***



###### 9.이미지에 링크

마크다운 이미지 코드를 링크 코드로 묶어 줍니다.

```
[![대체 텍스트](주소)](주소)
```

[![practice](/Users/nayeong-yun/Desktop/스크린샷 2020-04-23 오후 11.18.16.png)](https://naver.com)



***



###### 10.줄바꿈

```
* 줄바꿈을 하려면 문장의 끝에서 3번 띄워쓰기를 해야한다.___\\띄워쓰기  
이렇게

* 줄바꿈을 하려면 문장의 끝에서 3번 띄워쓰기를 해야한다.   
이렇게

```

* 줄바꿈을 하려면 문장의 끝에서 3번 띄워쓰기를 해야한다.   
이렇게
* 줄바꿈을 하려면 문장의 끝에서 3번 띄워쓰기를 해야한다.   이렇게

