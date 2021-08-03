# CSS

## 기본문법과 선택자의 역활
### 1. 기본 문법

```css
선택자{
    속성: 값;
    속성: 값;
}
```

### 2. 선택의 역활
    선택자는 HTML에 스타일을 적용하기 위해 HTML의 특정한 요소를 선택하는 사인.

```html
<div>
    <h1>제목</h1>
    <p>본문</p>    
```

```css
    h1{
        color:red;
    }
    p{
        color: blue;
    }
```

## 속성과 값
    속성과 값은 글자색은 무엇, 넓이는 얼마, 여백은 얼마 등을 지정

```css
div{
    color: red; /* 글자색은 빨강 */
    font-size: 20px; /* 글자 크기는 20px */        
}
```

## 선언 방식
### 1. 인라인 선언 방식(선택자가 없음)

```html
<div style="color: red">태그에 직접 작성1</div>
```

### 2. 내장 선언 방식

```html
<head>
    <style>
        div{
            color: red;
        }
    </style>
</head>
<body>
    <div>HTML에 적용됨</div>
    <div>HTML에 적용됨</div>
    <div>HTML에 적용됨</div>
</body>
```

### 3. 외부에서 불러오기
```html
<head>
    <link rel = "stylesheet" href="/css/main.css">
</head>
<body>
    <div>외부에서 불러오기</div>
<body>
```
```css
/* main css */
div{
    color: red;
}
```

## 선택자
### 1. 태그로 찾기
    선택자를 입력하는 부분에 적용하려는 태그의 이름 입력

```css
/* <h1> 글자 빨강 */
h1{
    color: red;
}
```
태그의 이름만 가지고는 특정하기가 어려움

### 2. 클래스로 찾기
```css
/* class="title"을 글자색 빨강 */
.title{
    color: red;
}
.main-text{
    color:blue;
}
```
```html
 <h1 class="title">제목1</h1> <!--얘만 빨강임 -->
 <h1>제목2</h1>
 <h1>제목3</h1>
 <h1>제목4</h1>
 <p class="text">본문</p> <!--얘만 파랑임 -->
 <p>본문</p>
 <p>본문</p>
```

 ## 속성
 ### 크기
 1. width (가로)
 ```css
 div{
     width: 300px;
 }
 ```

 2. height (세로)
 ```css
 div{
     height: 200px;
 }
 ```

 3. font-size (글자크기)
 ```css
 p{
     font-size: 16px;
 }
```

### 여백
1. margin (바깥 여백)
```css
div{
    margin: 20px;
}

.content{
    margin-top: 12px;
    margin-right: 5px;
    margin-bottom: 12px;
    margin-left: 5px;
}
```


2. padding (내부 여백)
```css
div{
    padding: 15px;
}

.content{
    padding-top: 12px;
    padding-right: 5px;
    padding-bottom: 12px;
    padding-left: 5px;
}
```


### 색상
1. color 
2. background
```css
div{
    color:red;
    background:pulm;
}
```

