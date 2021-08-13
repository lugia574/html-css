# @media
    다양한 미디어 유형이나 장치에 따라, 서로 다른 스타일 규칙을 적용

```css
@media 미디어타입 and (미디어 특성){
    css 코드
}

```
```css
@media screen and (max-width: 1200px) {
    body{
        color: red;
    }
}
```
>스크린이 max-width 1200px 까지 body color 는 red 다.

## 1. 미디어 타입
타입 | 의미 | 기본값 
--: | :---: | --: 
`all` | 모든 미디어 타입에 적용(생략 가능) | `all` 
`screen` | 컴퓨터 화면, 타블렛, 스마트폰 등 
`print` | 인쇄 전용 | 거의 안씀 ㅋ

## 2. 미디어 특성
타입 | 의미 
--: | :---: 
`width` | 뷰포트 가로 너비 
`max-width` | 뷰포트 최대 가로 너비(이하) 
`min-width` | 뷰포트 최소 가로 너비(이상)
`height`| 뷰포트 세로 너비
`max-height`| 뷰포트 최대 세로너비 (이하)
`min-height`| 뷰포트 최소 세로너비 (이상)
`orientation`| 뷰포트 방향(portrait,landscape)
기타| 다른 특성들..

