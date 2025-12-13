# 1만시간의 법칙

일만시간의 법칙 반응형 페이지 구현

## 구현 포인트

### 시멘틱 마크업

HTML5 시멘틱 태그 `section` `footer` `aside` `form` 등을 적극 활용하여 웹 접근성을 높였습니다.

### CSS 변수 (:root) 활용

color, box-shadow 등을 CSS 변수로 지정해 유지보수에 용이합니다.

## 구현 과정

### 모바일 레이아웃 구성

접근성이 높은 모바일 비율에 맞춰 구성

1. body 전체 padding 값 부여
2. `section` `footer` `aside` 에 width 100% 지정
3. `section` `footer` `aside` 자식요소에 `flex`, `grid` 부여

### media query 적용

가로형 태블릿 화면, 데스크탑 두가지 단계의 media query 적용
