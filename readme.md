# purpose : practice html, css, js, jquery, ajax, vuejs for final project

# start date : 2023. 03. 22

# ui, ux, psuedo class, transform, transition

# DAY 1(230322)

# 세미프로젝트 문제점(UI 한정)

# A조 - 양식 통일을 진행했음 but, 표준이 잘 지켜지지 않음

# B조 - 표준 설립 x

# UI팀

# - CSS 등 표준을 설립, 기본 양식 제공, 기능 구현을 좀 더 쉽게 처리

# - 이후 요청사항 처리 위주로 진행

# 1. transition : css속성값이 변할 때 속성값의 변화가 일정시간에 걸쳐 일어나도록 처리하는 것

# => transition은 자동으로 발동되지 않고 js의 부수적인 액션에 의해서만 발동, 혹은 pseudo-class를 통해 발동

# (1) transition-duration : 일어나는 지속시간을 초단위로 지정

# (2) timing-function : 효과를 위한 수치함수 지정

# -- timing function 5가지

# ==> ease : 기본값(느리게 시작 --> 점점 빨라짐 --> 느려지면서 종료)

# ==> linear : 일정한 속도로 계속감

# ==> ease-in : 느리게 시작하다가 일정 속도에 다다르면 그대로 등속운동

# ==> ease-out : 일정속도로 시작해서 점점 느려짐

# ==> ease-in-out : 느리게 시작해서 느려지면서 종료

# (3) delay : 시작하는 사이에 대기하는 시간 설정

# (4) property : 대상 속성 지정

# -- property의 대상이 되는 속성들

# ==> width, height, max-width, max-height, min-width, min-height

# ==> padding, margin

# ==> border-color, border-width, border-spacing

# ==> background-color, background-position

# ==> top, left, right, bottom

# ==> color, font-size, font-weight, letter-spacing, line-height, text-indent, text-shadow, vertical-align, word-spacing

# ==> opacity, outline-color, outline-offset, outline-width, visibility, z-index

# (5) transition(shorthand syntax) : 트랜지션 프로퍼티 한번에 지정하기

# -- transition 효과 중 layout에 영향을 크게 주는 효과는 사용을 지양해야함

# -- layout에 직접적 영향을 주는 속성들

# ==> width, height, padding, margin, border, display, position, float, overflow

# (6) transform : html 요소의 모양, 크기, 위치 등을 제어하는 속성

# -- 요소의 움직임, 회전, 크기변경, 기울임 등의 동작을 한꺼번에 적용

# -- 2D 트랜스폼, 3D 트랜스폼

# -- 2D transform 메소드

# ==> translate : 현재 위치에서 해당 요소를 주어진 x, y축 거리만큼 이동

# ==> rotate : 해당 요소를 주어진 각도만큼 시계(양수)/ 반시계(음수) 방향으로 회전

# ==> scale : 해당 요소의 크기를 주어진 배율만큼 늘리거나 줄이는 메소드, 1보다 크면 확대, 작으면 축소

# ==> skew : 해당 요소를 주어진 각도만큼 x/y축 방향으로 기울임, skewX/ skewY라는 응용메소드 활용 가능

# ==> matrix : 트랜스폼 숏핸드 문법 /ex. skewX(), skewY(), skewX(), skewY(), translateX(), translateY()

# ---------------------------------------------------------------------------------------------------------

# DAY 2(230323)

# 2. Animation 효과

# => 요소의 현재 스타일을 다른 스타일로 천천히 변화시키는 속성

# => 애니메이션은 css 스타일 + 복수의 @keyframes로 이루어짐

# => 트랜지션, 트랜스폼으로 어느정도의 애니메이션 효과는 가능 but 제한적

# => 트랜지션은 이벤트같은 부수적인 액션에 의해서만 발동

# (1) Transition vs Animation

# -- 트랜지션은 단순히 요소의 속성 변화에 초점을 둠

# -- 애니메이션은 하나의 스토리처럼 세부적인 움직임을 시간 흐름 단위로 제어 가능(재생, 정지, 반복)

# (2) Animation Property

# -- animation-name : 애니메이션의 이름 지정

# ㄴ> 요소에 부여되는 스타일과 애니메이션의 연결

# -- animation-duration : 한 사이클의 애니메이션에 소요되는 초단위 밀리초단위 시간지정

# -- animation-timing-function : 효과를 위한 타이밍 지정

# ㄴ> 트랜지션의 속성값들과 같은 논리(ease, linear, ease-in, ease-out, ease-in-out)

# -- animation-delay : 애니메이션 시작 대기시간 지정

# -- animation-iteration-count : 재생횟수 지정

# -- animation-fill-mode : 애니메이션 미 실행 시 요소의 스타일 지정

# -- animation-play-state : 애니메이션 재생상태 지정

# ㄴ> paused, running

# -- animation-direction : 진행방향 설정

# ㄴ> 정방향 : alternate ( 진행방향을 애니메이션이 반복될 때마다 계속 변경)

# ㄴ> 역방향 : reverse

# -- animation : 애니메이션 숏핸드(속성 한꺼번에 저장하기)

# 3. Layout 심화(반응형)

# => 과거 : 테이블로 레이아웃

# => 최근 : 플렉서블 박스, 그리드, 시멘틱 태그

# (1) 반응형 웹 앱

# -- 스마트폰의 등장으로 장치에 따라 제공되는 화면의 크기가 달라야함

# -- viewport : 화면에 보이는 브라우저 창 만큼을 의미
