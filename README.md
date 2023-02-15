# HTML

<태그>내용</태그>

종료(닫힌) 태그가 없는 경우를 빈태그라고 함

<태그 /> 를 사용하면 더 안전함

<태그 속성 = “값”> 내용 </태그>

기능의 확장

<img src = “” alt = “” />

대부분의 빈태그들은 속성과 값을 사용

꼭 필요한 속성을 필수속성 이라고함

## 글자와 상자

요소가 화면에 출력되는 특성

인라인(Inline) 요소 : 글자를 만들기 위한 요소들

블록(Block) 요소 : 상자(레이아웃)를 만들기 위한 요소들

### **인라인 요소**

<span></span> 대표적인 인라인 요소

본질적으로 아무것도 나타내지 않는, 콘텐츠 영역을 설정하는 용도

요소가 수평으로 쌓임

줄 바꿈 행위가 띄어쓰기로 사용됨

포함한 콘텐츠 크기만큼 자동으로 **줄어듬 (줄어드려고 함)**

가로 사이즈와 세로 사이즈를 지정할 수 없음

위, 아래는 여백을 정상적으로 추가할 수 없음

자식요소로 블록 요소를 사용할 수 없음 (인라인 요소는 가능)

### 블록 요소

<div></div> 대표적인 블록 요소

본질적으로 아무것도 나타내지 않는, 콘텐츠 영역을 설정하는 용도

요소가 수직으로 쌓임

부모 요소의 크기만큼 자동으로 **늘어감 (가로 너비는 늘어나려고 함, 세로 너비는 줄어드려고 함)**

가로 세로 사이즈를 지정할 수 있음

상하좌우 여백 정상적으로 추가할 수 있음

자식요소로 블록 요소, 인라인 요소도 넣을 수 있음

## 핵심 요소

<div></div> **블록 요소** / 특별한 의미가 없는 구분을 위한 요소 (Division)

<h1></h1> **블록 요소** / 제목을 의미하는 요소 (Heading) 1~6번까지 있음 **(작을수록 중요)**

<p></p> **블록 요소** / 문장을 의미하는 요소 (Paragraph)

<img src**(필수속성)** = “(경로)” alt**(필수속성)** = “(이름)” /> **인라인 요소** / 

이미지를 삽입하는 요소 (Image)

<ul> **블록 요소** / 순서가 필요없는 목록의 집합을 의미 (Unordered List)

<li></li> **블록 요소** / 목록 내 각 항목 (List Item)

</ul>

<a href = “(경로)”>내용</a> **인라인 요소** / 다른,같은 페이지로 이동하는 

하이퍼링크를 지정하는 요소(Anchor)

target = “_blank” 속성을 넣으면 새 탭에 열림

<span></span> **인라인 요소** / 특별한 의미가 없는 구분을 위한 요소

<br/> **인라인 요소** / 줄바꿈 요소 (Break)

<input type = “(입력받을 데이터 타입)” /> **인라인 요소, 블록 요소** (수평으로 쌓이는 특징이 있지만 

위아래 좌우 여백과 크기를 정할수 있음) / 사용자가 데이터를 입력하는 요소

value = “미리 입력된 값(데이터)”

placeholder = “사용자가 입력할 값(데이터)의 힌트”

disabled =  입력 요소 비활성화

<label> **인라인 요소** / 라벨 가능 요소(input)의 제목

<input type = “checkbox” /> Apple 

checked = 체크박스 입력 요소 체크됨

<input type = “radio” name = “(그룹)” /> 체크 여부를 그룹에서 1개만 입력 받음

</label> 

<table> **테이블 요소** / 표 요소 행(Row)과 열(Column)의 집합

<tr> 행(Row)을 지정하는 요소 (Table Row)

<td>내용</td> 열(Column)을 지정하는 요소(Table Data)

</tr>

</table>

## 전역속성

body 태그에 사용하는 모든 태그에 사용가능한 속성

<태그 title = “내용”></태그>  / 마우스를 올렸을 때 나타나는 내용 (요소의 정보나 설명)

<태그 style = “스타일”></태그> / 요소에 적용할 스타일(CSS)를 지정

<태그 class = “이름”></태그> / 요소를 지칭하는 중복 가능한 이름

css 선택자를 이용할때 .을 붙여 class를 표시함 

<태그 id = “이름”></태그> / 요소를 지칭하는 고유한 이름

#을 이용해 id를 선택

<태그 data-이름=”데이터”></태그> / 요소에 데이터를 지정

# CSS

선택자 { 속성: 값; }

선택자 : 스타일(CSS)을 적용할 대상 (Selector)

## CSS 선언 방식

### 내장 방식 :

<style></style>의 내용으로 스타일을 작성하는 방식

html 내부에다가 작성

별도의 css 파일 필요 없음

나중에 복잡해지기 때문에 권장 x

### 인라인 방식 :

요소의 style 속성에 직접 스타일을 작성하는 방식 ( 선택자 없음 )

유지 보수하는데 악영향을 미치기때문에 권장 x

### 링크 방식 :

<link />로 외부 css 문서를 가져와서 연결하는 방식

병렬 방식

### @import 방식 :

css의 @import 규칙으로 css문서 안에서 또 다른 css 문서를 가져와 연결하는 방식

직렬로 연결 처음 연결된 css가 끝날때까지 연결이 안됨

지연시키는 용도로 사용가능

# 선택자


### 기본 / 전체 선택자 (Universal Selector)

**모든 요소**를 선택

* { 

}

### 기본 / 태그 선택자(Type Selector)

**태그 이름이 ABC인 요소** 선택

li(태그이름) {

}

### 기본 / 클래스 선택자(Class Selector)

HTML **class 속성의 값이 ABC인 요소** 선택

.orange(클래스이름) {

}

### 기본 / 아이디 선택자(ID Selector)

HTML **id 속성의 값이 ABC인 요소** 선택

#oragne(id 값) {

}

**복합 선택자는 마지막에 있는 선택자를 찾아내는 개념**

### 복합 / 일치 선택자(Basic Combinator)

선택자 ABC와 XYZ를 **동시에 만족**하는 요소 선택

span(태그).orange(클래스) {

}

### 복합 / 자식 선택자(Chile Combinator)

선택자 ABC의 **자식 요소** XYZ 선택

ul > .orange {

}

### 복합 / 하위(후손) 선택자 (Descendant Combinator)

선택자 ABC의 하위 요소 XYZ 선택

**‘띄어쓰기’가 선택자의 기호!**

div .orange {

} 일반적으로 자식선택자보다 하위선택자를 많이 씀

### 복합 / 인접 형제 선택자(Adjacent Sibling Combinator)

선택자 ABC의 다음 형제 요소 XYZ **하나를** 선택

.orange + li {

}

### 복합 / 일반 형제 선택자(General Sibling Combinator)

선택자 ABC의 다음 형제 요소 XYZ **모두를** 선택

.orange ~ li {

}

# 가상 클래스 선택자(Pseudo-Classes)

### HOVER

선택자 ABC 요소에 **마우스 커서가 올라가 있는 동안** 선택.

:hover { 

}

### ACTIVE

선택자 ABC 요소에 **마우스를 클릭하고 있는 동안** 선택

:active {

}

### FOCUS

선택자 ABC 요소가 **포커스되면** 선택

:focus {

} 

focus가 가능한 요소들에만 작동함 ( 대표적으로 input 요소 )

tabindex =”-1” 속성을 넣으면 작동할수있음 ( 권장 x )

### FIRST CHILD

선택자 ABC가 형제 요소 중 첫째라면 선택

:first-child {

}

### LAST CHILD

선택자 ABC가 형제 요소 중 막내라면 선택

:last-child {

}

### NTH CHILD

선택자 ABC가 형제 요소 중 (n)째라면 선택

:nth-child(숫자) {

}

n이라는 키워드가 있는데 0부터 시작 2n = 2 * n  2의 배수 2n +1은 홀수

### 부정 선택자(Negation) / NOT

선택자 XYZ가 아닌 ABC 요소 선택

:not(XYZ) {

}

## 가상 요소 선택자(Pseudo-Elements)

### BEFORE

가상의 인라인 요소

선택자 ABC 요소의 **내부 앞**에 내용(Content)을 삽입

::before {

content: “” ;

}

### AFTER

선택자 ABC 요소의 **내부 뒤**에 내용(Content)을 삽입

::after {

content: “”;

}

Content 속성과 무조건 함께 써야함

# 속성 선택자(Attribute)

### ATTR

속성 ABC를 포함한 요소 선택

[disabled(속성)] {

}

### ATTR = VALUE

속성 ABC를 포함하고 값이 XYZ인 요소 선택

[type(속성) = “password(값)”] {

}

## 스타일 상속

상속되는 CSS 속성들

모두 글자 / 문자 관련 속성들

# 속성

## 박스 모델

## 요소의 가로/세로 너비

### **width, height**

auto / 브라우저가 너비를 계산

단위 / px, em, vw등 단위로 지정

### **max-width, max-height**

none / 최대 너비 제한 없음

auto / 브라우저가 너비를 계산

단위 / px, em, vw 등 단위로 지정

### **min-width, min-height**

0 / 최소 너비 제한없음

auto / 브라우저가 너비를 계산

단위 / px, em, vw 등 단위로 지정

## 단위

px / 픽셀

% / 상대적 백분율

em / 요소의 글꼴 크기

rem / 루트(최상위) 요소(html)의 글꼴 크기

vw / 뷰포트 가로 너비의 백분율

vh / 뷰포트 세로 너비의 백분율

### margin (음수 사용 가능)

요소의 **외부** 여백(공간)을 지정하는 **단축 속성**

0 / 외부 여백 없음

auto / 브라우저가 여백을 계산 (가운데 정렬에 활용)

단위 / px, em, vw 등 단위로 지정

% / 부모 요소가 가로 너비에 대한 비율로 지정

-top, -bottom, -left, -right

top,bottom / left,right

top / left,right / bottom

top / right / bottom / left

### padding (요소의 크기가 커짐)

요소의 내부 여백(공간)을 지정하는 단축 속성

0 / 내부 여백 없음

단위 / px, em, vw 등 단위로 지정

% / 부모 요소의 가로 너비에 대한 비율로 지정

## border (요소의 크기가 커짐)

요소의 **테두리 선**을 지정하는 **단축** 속성

: 선-두께(border-width) 선-종류(border-style) 선-색상(border-color)

### border-width /요소 테두리 선의 두께

medium / 중간 두께

단위 / px, em, % 등 단위로 지정

### border-style / 요소 테두리 선의 종류

none / 선 없음

solid / 실선(일반 선)

dashed / 파선

### border-color

black / 검정색

색상 / 선의 색상

transparent / 투명

### border-radius / 요소의 **모소리를** **둥글게 깎음**

0 / 둥글게 없음

단위 / px, em, vww 등 단위로 지정

시계 방향으로 순서

### box-sizing / 요소의 **크기 계산 기준**을 지정

content-box / 요소의 내용(content)으로 크기 계산

border-box / 요소의 내용 + padding + border로 크기 계산

### overflow ( 단축 속성 )

요소의 크기 이상으로 **내용이 넘쳤을 때, 보여짐을 제어**하는 단축 속성

visible / 넘친 내용을 그대로 보여줌

hidden / 넘친 내용을 잘라냄

scroll / 넘친 내용을 잘라냄, 스크롤바 생성

auto / 넘친 내용이 있는 경우에만 잘라내고 스크롤바 생성

### display / 요소의 화면 **출력(보여짐)** 특성

block / 상자(레이아웃) 요소

inline / 글자 요소

inline-block / 글자+상자 요소

flex / 플렉스 박스 (1차원 레이아웃)

grid / 그리드 (2차원 레이아웃)

none / 보여짐 특성 없음, 화면에서 사라짐

기타 / table, table-row, table-call 등..

### opacity

요소 **투명도**

1 / 불투명

0 / 완전한 투명

## 글꼴

### font-style / 글자의 기울기

normal / 기울기없음

italic / 이텔릭체 ( 기울어짐 )

oblique / 기울어진 글자

### font-weight / 글자의 두께

normal, 400 / 기본 두께

bold, 700 / 두껍게

bolder / 상위 요소보다 더 두껍게

lighter / 상위 요소보다 더 얇게

100 ~ 900 / 100단위의 숫자 9개, normal과 bold 이외 두께

### font-size / 글자의 크기

16px / 기본 크기

단위 / px, em, rem등 단위로 지정

### line-height / 한 줄의 높이, 행간과 유상(글자 부분은 가운데 정렬됨)

normal / 브라우저의 기본 정의를 사용

숫자 / 요소의 글꼴 크기의 배수로 지정

단위 / px, em, rem 등의 단위로 지정

### font-family / 글꼴(서체) 지정

: 글꼴1, “글꼴2(후보)”, … 글꼴계열;

띄어쓰기 등 특수문자가 포함된 글꼴 이름은 큰 따옴표로 묶어야 함

## 문자

### color / 글자의 색상

rgb(0, 0, 0) / 검정색

색상 / 기타 지정 가능한 색상

### text-align / 문자의 정렬 방식

left / 왼쪽정렬

right / 오른쪽 정렬

center / 가운데 정렬

justify / 양쪽 정렬

### text-decoration / 문자의 장식(선)

none / 장식 없음

underline / 밑줄

overline / 윗줄

line-through / 중앙 선

### text-indent / 문자 첫 줄의 들여쓰기

0 / 들여쓰기 없음

단위 / px, em, rem등 단위로 지정

음수를 사용할 수 있음 (내어쓰기)

## 배경

### background-color / 요소의 배경 색상

transparent / 투명함

색상 / 지정 가능한 색상

### background-image / 요소의 배경 이미지 삽입

none / 이미지 없음

url(”(경로)”) / 이미지 경로

### background-repeat / 요소의 배경 이미지 반복

repeat / 이미지를 수직, 수평 반복

repeat-x / 이미지를 수평 반복

repeat-y / 이미지를 수직 반복

no-repeat / 반복 없음

### background-position / 요소의 배경 이미지 위치

0%0% / 0%~100% 사이 값

방향 / top, bottom, left, right, center 방향 (방향1, 방향2)

단위 / px, em, rem 등 단위로 지정 (x축, y축)

### background-size / 요소의 배경 이미지 크기

auto / 이미지 실제 크기

단위 / px, em, rem 등 단위로 지정

cover / 비율을 유지, 요소의 더 넓은 너비에 맞춤

contain / 비율을 유지, 요소의 더 짧은 너비에 맞춤

### background-attachment / 요소의 배경 이미지 스크로로 특성

scroll / 이미지가 요소를 따라서 같이 스크롤

fixed / 이미지가 뷰포트에 고정, 스크롤x

local / 요소 내 스크롤 시 이미지가 같이 스크롤

## 배치

### position / 요소의 위치 지정 기준

static / 기준 없음

relative / 요소 자신을 기준

absolute / 위치 상 부모 요소를 기준

fixed / 뷰포트(브라우저)를 기준 

absolute 를 사용할때 위치 상 부모 요소를 기준으로 하기 때문에 부모 요소에 relative 가 필요

fixed는 뷰포트를 기준으로 하기때문에 스크롤이 내려가도 그 위치에 있음

### top, bottom, left, right 사용

### 요소 쌓임 순서(Stack order)

어떤 요소가 사용자와 더 가깝게 있는지(위에 쌓이는지) 결정

1. 요소에 position 속성의 값이 있는 경우 위에 쌓임.(기본값 static 제외)
2. 1번 조건이 같은 경우, z-index 속성의 숫자 값이 높을 수록 위에 쌓임.
3. 1번과 2번 조건까지 같은 경우, HTML의 다음 구조일 수록 위에 쌓임.

### Z-index / 요소의 쌓임 정도를 지정

auto / 부모 요소와 동일한 쌓임 정도

숫자 / 숫자가 높을 수록 위에 쌓임

**position 속성의 값으로 absolute, fixed로 지정된 요소는** 

**display 속성이 block으로 변경됨**

## 플렉스(정렬)

### display / Flex Container의 화면 출력(보여짐) 특성

flex / 블록 요소와 같이 Flex Container 정의

inline-flex / 인라인 요소와 같이 Flex Container 정의

### flex-direction / 주 축을 설정

row / 행 축 (좌 > 우)

row-reverse / 행 축 (우 > 좌)

column / 열 축 (위 > 아래)

column-reverse / 열 축 (아래 > 위)

### flex-wrap / Flex-items 묶음(줄 바꿈) 여부

nowrap / 묶음(줄 바꿈) 없음

wrap / 여러 줄로 묶음

### justify-content / 주 축(수평)의 정렬 방법

flex-start / Flex Items를 시작점으로 정렬

flex-end / Flex Items를 끝점으로 정렬

center / Flex Items를 가운데 정렬

### align-content / 교차 축(수직)의 여러 줄 정렬 방법

stretch / Flex Items를 시작점으로 정렬

flex-start / Flex Items를 시작점으로 정렬

flex-end / Flex Items를 끝점으로 정렬

center / Flex Items를 가운데 정렬

### align-items / 교차 축의 한 줄 정렬 방법

stretch / Flex Items를 교차 축으로 늘림

flex-start / Flex Items를 각 줄의 시작점으로 정렬

flex-end / Flex Items를 각 줄의 끝점으로 정렬

center / Flex Items를 각 줄의 가운데 정렬

## Flex-Items에 부여되는 Flex 속성

### order / Flex Item의 순서

0 / 순서 없음

숫자 / 숫자가 작을 수록 먼저

### flex-grow / Flex Item의 증가 너비 비율

0 / 증가 비율 없음

숫자 / 증가 비율

### flex-shrink / Flex Item의 감소 너비 비율

1 / Flex Container 너비에 따라 감소 비율 적용

숫자 / 감소 비율

### flex-basis / Flex Item의 공간 배분 전 기본 너비

auto / 요소의 Content 너비

단위 / px, em, rem 등 단위로 지정 ( 0을 쓰면 content 상관없이 비율을 맞춰줌)

## 전환

## transition : 속성명 지속시간(필수속성) 타이밍함수 대기시간;

### transition-property / 전환 효과를 사용할 속성 이름을 지정

all / 모든 속성에 적용

속성이름 / 전환 효과를 사용할 속성 이름 명시

### transition-duration / 전환 효과의 지속시간을 지정

0s / 전환 효과 없음

시간 / 지속시간(s)를 지정

### transition-timing-function / 전환 효과의 타이밍(Easing)함수를 지정

ease / 느리게 - 빠르게 - 느리게

linear / 일정하게

ease-in / 느리게 - 빠르게

ease-out / 빠르게 - 느리게

ease-in-out / 느리게 - 빠르게 - 느리게

### transition-delay / 전환 효과가 몇 초 뒤에 시작할지 대기시간을 지정

0s / 대기시간 없음

시간 / 대기시간(s)을 지정

## 변환

## transform: 변환함수1 변환함수2 변환함수3 … ;

## transform: 원근법 이동 크기 회전 기울임;

## 2D 변환 함수

### px

- translate(x,y) / 이동(x축, y축)
- translateX(x) / 이동(x축)
- translateY(y) / 이동(y축)

### 없음(배수)

- scale(x,y) / 크기(x축, y축)

### deg

- rotate(degree) / 회전(각도)
- skewX(x) / 기울임(x축)
- skewY(y) / 기울임(y축)

## 3D 변환 함수

### px

- perspective(n) / 원근법(거리)

### deg

- rotateX(x) / 회전(x축)
- rotateY(y) / 회전(y축)

### perspective / 하위 요소를 관찰하는 원근 거리를 지정

단위 / px 등 단위로 지정

속성은 관찰 대상의 부모에게 적용

함수는 관찰 대상에게 직접 적용한다

### backface-visibility / 3D 변환으로 회전된 요소의 뒷면 숨김 여부

visible / 뒷면 보임

hidden / 뒷면 숨김

## 그리드 (2차원 정렬)

### display:grid

grid-template-columns 행

grid-template-rows 열

grid-template-areas

grid-gap{

grid-column-gap

grid-row-gap

}

### grid cell

grid-column-start

grid-column-end

grid-row-start

grid-row-end

grid-area