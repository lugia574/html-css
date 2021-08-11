# Float
    요소를 좌우 방향으로 띄움 (수평 정렬)

## 1. 속성값
값 | 의미 | 기본값 
--: | :---: | --: 
`none` | 요소 띄움 없음 | 'non' 
`left` | 왼쪽으로 띄움 |
`right` | 오른쪽으로 띄움

## 2. float 해제
    flaot 속성이 적용된 요소의 주위로 다른 요소들이 흐르게 되는데
    이를 방지하기 위해 속성을 해제 해야함


### 해제 방법 3가지

#### 1. 형제 요소에 clear: (left, right, both) 추가하여 해제
```html
<div class = "float-left"></div>
<div class = "float-left"></div>
<div class = "next"></div>

```
```css
.foat-left{
    width: 100px;
    height: 100px;
    background: red;
    float: left;
}

.next {
    clear: both;
}

```

- 문제점 - 다음 형제 요소가 없음 해제를 못함 ㅋ

#### 2. 부모요소에 overflow: (hidden, auto) 추가하여 해제

```html
    <div class = "parent">
        <div class = "child"></div>
        <div class = "child"></div>
    </div>
```
```css
    .parent{
        overflow: hidden; /* auti */
    }

    .child{
        float: left
    }
```
- 문제점 - overflow는 float랑 아무 관련이 없는 편법임

#### 3. 부모요소에 clearfix 클래스 추가하여 해제 (**추천**)

- float 속성이 추가된 요소의 부모요소에 미리 지정된 clearfix 클래스 추가

```html
<div class="parent clearfix">
    <div class="child"></div>
    <div class="child"></div>
</div>
```
```css
.clearfix::after{
    content: "";
    clear: both;
    display: block; /* table */
}
.child{
    float: left;
}
```


```html
::after 를 쓰므로써

<div class="parent clearfix">
    <div class="child"></div>
    <div class="child"></div>
----------------------------
여기에 clear: both; 가 적용된다잉
</div>
```
**주의** 

    clearfix 내의 자식요소에는 무적권 float이 들어 있는 요소들만 있어야 한다


## 3. display 수정
    float 속성이 추가된 요소는 display 속성값이 대부분 block으로 수정됨
