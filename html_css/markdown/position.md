# Position
    요소의 위치 지정 방법의 유형(기준)을 설정

## 1. 속성값
값 | 의미 | 기본값 
--: | :---: | --: 
`static` | 유형(기준) 없음/ 배치 불가능 | `static` 
`relative` | 요소 자신을 기준으로 배치 |
`absolute` | 위치 상 부모요소를 기준으로 배치
`fixed` | 브라우저(뷰포트)를 기준으로 배치
`sticky` | 스코롤 영역 기준으로 배치

### 0. static
> 기본값 잘 안씀

<br>

### 1. relative
> 자기 자신을 스스로 기준으로 잡음 <br>
> 자기가 있었던 자리에서 기준으로 몇만큼 간다는 소리 <br>
> `relative`는 주변에 있는 형제 요소에 영향을 줌 <br>
> 고로 `relative` 에 속성값을 직접적으로 주는건 별로다~

<br>

### 2. absolute
> 부모 요소를 기준으로 배치 (위치 상의 부모) <br>
> 요거랑 relative 를 젤 마니 쓰는듯

<br>

### 3. fixed
> 광고 배너 같은게 마니 쓰는듯 <br>
> 아님 헤더부분에 쓸 수 있음

<br>

### 4. sticky
> top, left 등의 속성값이 한개 이상이 있어야 함 <br>
> IE 지원 불가 <br>



## 요소 쌓임 z 축
    1. static을 제외한 position 속성의 값이 있을 경우 가장 위에 쌓임
    2. position 이 모두 존재 한다면 z-index 속성의 숫자 값이 높을 수록  위에 쌓임
    3. position 속성의 값이 있고, z-index속성의 숫자값이 같다면
    html 의 마지막 코드일 수록 위에 쌓임


## display 수정
    absolute, fixed 속성 값이 적용된 요소는 display 속성의 값이 대부분 block으로 수정됨

