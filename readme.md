# purpose : practice html, css, js, jquery, ajax, vuejs for final project

# start date : 2023. 03. 22

# ui, ux, psuedo class, transform, transition

# day1

# 세미프로젝트 문제점(UI 한정)

# A조 - 양식 통일을 진행했음 but, 표준이 잘 지켜지지 않음

# B조 - 표준 설립 x

# UI팀

# --> CSS 등 표준을 설립, 기본 양식 제공, 기능 구현을 좀 더 쉽게 처리

# --> 이후 요청사항 처리 위주로 진행

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

# => transition 효과 중 layout에 영향을 크게 주는 효과는 사용을 지양해야함

# --layout에 직접적 영향을 주는 속성들

# ==> width, height, padding, margin, border, display, position, float, overflow

# transform : html 요소의 모양, 크기, 위치 등을 제어하는 속성

# => 요소의 움직임, 회전, 크기변경, 기울임 등의 동작을 한꺼번에 적용

# => 2D 트랜스폼, 3D 트랜스폼

# 2D transform 메소드

# => translate : 현재 위치에서 해당 요소를 주어진 x, y축 거리만큼 이동

# => rotate : 해당 요소를 주어진 각도만큼 시계(양수)/ 반시계(음수) 방향으로 회전

# => scale : 해당 요소의 크기를 주어진 배율만큼 늘리거나 줄이는 메소드, 1보다 크면 확대, 작으면 축소

# => skew : 해당 요소를 주어진 각도만큼 x/y축 방향으로 기울임, skewX/ skewY라는 응용메소드 활용 가능

# => matrix : 트랜스폼 숏핸드 문법 /ex. skewX(), skewY(), skewX(), skewY(), translateX(), translateY()
