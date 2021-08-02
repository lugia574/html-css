# 마크다운 문법 학습하기

## 마크다운 소개

## 마크다운 문법

### 제목

### 강조
*별표를 이용한 이텔리체* <br> 
_언더바를 이용한 이텔리체_

**_두껍게 별표 이텔리체_** <br>
__*두껍게 언더바 이텔리체*__

*동해물*과 **백두산**이 ~~마르고~~ <u>닳도록</u>

### 목록
오엘, 유엘 태그로 변환됨

#### 라면 끓이는 법
1. 라면을 구입
1. 물을 끓인다
1. 스프를 넣는다.
1. 면을 넣는다.
1. 맛잇게 끓인다.
1. 맛있게 먹는다.
1. 맛있게 설거지를 한다.


#### 과일 목록

- 사과
- 파인애플
- 딸기
- 오렌지
- 망고

### 링크
[GooGLE](https://google.com) <br>
[NAVER](https://naver.com "링크 설명(title)을 작성하세요.")<br>
[상대적 참조](../user/login)

저는 [구글](https://google.com) 그 자체 입니다.

[네이버](https://naver.com)에 [마크다운(Markdown)](https://heropy.blog/2017/09/30/markdown/)을 검색하세용.

[GitHub 참조 링크][1]

https://google.com <br>
바로 링크 걸어버리기~



[1]: https://github.com

### 이미지

![대체텍스트](https://post-phinf.pstatic.net/MjAyMTA3MjlfMzMg/MDAxNjI3NTQ1NjgwOTY5.hr_y6uisUgMifXMee_ZPxjSNCfAowZGCGisG2tni46Qg.nTYDZaKbm7Me7dfGwAx0wFJjBDcPyp8nJgseTvRdX3wg.JPEG/44114.jpg?type=w1200)

이미지 누르면 링크로 가게 하는법
[![대체텍스트](https://post-phinf.pstatic.net/MjAyMTA3MjlfMTYg/MDAxNjI3NTQ1NjgwOTQ5.s9r0QQcgQW8UOu5M1Yjl7KJMAgn5qbgRuUHqDZ2BUAYg.e30BDoFDkZm6mxV8RVJWzFeHeWKoEn9H3n4Yk_yADkEg.JPEG/55555.jpg?type=w1200)](https://post.naver.com/viewer/postView.naver?volumeNo=32068790&memberNo=31724756)


### 코드 강조
`<pre>`, `<code>` 태그로 변환됨

#### 인라인 코드 강조
`background` 혹은 `background-img` 속성으로 요소에 배경 삽입 가능

#### 블록 코드 강조
```html 
<div id="hi" style="color:red;"></div>
<span> 안녕녕 </span>
```

```css 
#markdown{
    position:absolute;
    margin: 10px;
    width: 150px;
}

```

```js 
function hello(){
    return {};
}
```

### position의 값
값 | 의미 | 기본값 
--: | :---: | --: 
`static` | 유형(기준) 없음/ 배치 불가능 | 'static' 
`relative` | 요소 **자신**을 기분으로 배치 |
`absolute` | 부모 요소를 기준으로 배치
`fixed` | 브라우저 창을 기준으로 배치


### 인용문
> 요호호호호
>> 오효효효효수 해버릴라 <br>
>> 그럴까요~
>>> 슈슈슉슈수슉


### 원시 HTML
<blockquote>원시 저그인가?</blockquote>
<br>
<img src="https://post-phinf.pstatic.net/MjAyMTA3MjlfODUg/MDAxNjI3NTQ0MzM4MDI0.mymY-rU3TsgnaDspF5wsWs34d66yJmRG--kR-z0RCh4g.Elna33LKvugJLzVj7STgpCOO8bHgoz2fgEOFO3DVBBgg.JPEG/%EC%84%A4%ED%91%9C7777.jpg?type=w1200" alt="커여운 표범" width="500"
>

### 수평선
---
엄청나군

***
이렇게도 된다네
___
요호호호

### 줄 바꿈
- 뛰어 쓰기 두번을 쓰면 됨
- 근데 안될수도 있으니까 `<br>` 태그를 쓰자
---

동해물과 백두산이 마르고 닳도록  
하느님이 보우하사 우리나라 만세  
무궁화 삼천리 화려 강산  
대한 사람 대한으로 길이 보전하세  

