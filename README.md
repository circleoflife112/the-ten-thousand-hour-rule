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
2. `section` `footer` `aside` 에 고정값(360px) 지정
3. `section` `footer` `aside` 내부에서 `flex`, `grid` 등을 활용해 반응형

### media query 적용

와이드 태블릿 화면, 데스크탑 두가지 단계의 media query 적용
