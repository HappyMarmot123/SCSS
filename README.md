# Why use SCSS (SASS + CSS)?

## 컴포넌트 단위 웹 개발 트렌드에 굉장히 적합한 방식을 사용한다

## 마멋의 개인적 견해

SCSS는 결과물을 최종적으로 CSS으로 컴파일됩니다.
그렇기에 SCSS에 익숙하지 않은 사람들도 바닐라 CSS 문법으로 대체할 수 있습니다.
마치 타입스크립트 처음 써보는 사람에 any를 남발하는 것과 같습니다(?)
SASS/SCSS는 필수가 아니지만 큰 규모의 프로젝트에서는 굉장한 생산성을 보여줍니다.

## 변수(Variables) 사용 가능

$primary-color: #3498db;
$font-size: 16px;

## 직관적인 중접 스타일

.nav {
background-color: #333;
ul {}
li {}
}

## 재사용 가능한 믹스인

@mixin border-radius($radius) {
-webkit-border-radius: $radius;
-moz-border-radius: $radius;
border-radius: $radius;
}
.box {
@include border-radius(10px);
}

## 스타일 상속

.message {
padding: 10px;
background-color: #f9f9f9;
}
.success {
@extend .message;
border-left: 5px solid green;
}

## scss파일 임포트 지원

// \_variables.scss
$primary-color: #333;

// main.scss
@import 'variables';
body { color: $primary-color; }

## 조건문 및 반복문 사용 가능

# How do i get Start

Use VSC Extension (Live Sass Compiler)
