# 1만시간의 법칙

일만시간의 법칙 반응형 페이지 구현

## 동기

1. 코드를 어떻게 작성했는지 나눌 수 있는 좋은 기회
2. 상품 - 제주도 여행을 눈독들이는 가족들

## 느낀점 (수확)

1. 시멘틱 마크업에 따른 구조적인 코드 작성을 배웠습니다.
   - `heading` 태그의 사용법
   - `section` `article` `aside` 등 사용
2. 디자이너와의 협업을 간접적으로나마 경험
3. 디자이너 & 프론트엔드 개발자가 개인적인 목표 - 디자인부터 구조적이어야 웹 구현에 용이하다는 점 깨달음

## 구현 포인트

모바일을 기준으로 데스크톱 화면까지 자연스러운 반응형 웹페이지 구현

### 시멘틱 마크업

HTML5 시멘틱 태그 `section` `footer` `aside` `form` 등을 적극 활용하여 웹 접근성을 높였습니다.

### CSS 변수 (:root) 활용

color, box-shadow 등을 CSS 변수로 지정해 유지보수에 용이합니다.

### CSS 클래스 네이밍 : 케밥 케이스(kebab-case) 적용

통일감 있는 클래스 작성법으로 혼란을 줄입

## 구현 과정

### 모바일 레이아웃 구성

접근성이 높은 모바일 비율에 맞춰 구성

1. body 전체 padding 값 부여
2. `section` `footer` `aside` 에 width 100% 지정
3. `section` `footer` `aside` 자식요소에 `flex`, `grid` 부여

### media query 적용

가로형 태블릿 화면, 데스크탑 두가지 단계의 media query 적용

section 안에 h(heading)요소가 하나만 들어가는 걸 권장드립니다,
section 이 나눠지면 h(heading)요소는 필수입니다.

1. display : none; >> 하지 마세요. 스크린 리더에서 읽을 수 없습니다.
2. padding or margin: -99999 해서 : 그러나 메모리 부하 : 옛날

3. naver 쓰는 방법 : .blind > 클래스명이 조금 구식이지만 이 클래스에 있는 속성 그대로 베껴 쓰면 됩니다.

4. screen reader only
   accecibiltiy
