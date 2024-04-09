html 파일의 요소들을 디자인하고 색을 넣고..하는 역할
이름{ 속성 } 의 구조
이름=선택자

선택자 {
    속성 : 값;
    속성 : 값;
}

@import "~";
@media (min-width: 너비 설정) { };
/* 주석 */

html body의 선택자 이름으로
css에서 그것의 속성을 바꿔준다!

- 예를 들면
html 파일에 이 버튼을 만들면
    <button> 버튼</button>
이것의 속성을 css에서 바꿀 수 있다
    button { 
    background-color: paleturquoise;
    ... 다른 속성들
    }

- 다른 경우 html
    <button color="orange"> 버튼</button>
이 속성을 바꾸고 싶으면
    button[color="orange"]{
    border-color: rgb(252, 105, 14);
    ... 다른 속성들
    }
혹은 속성 선택자 [ ]을 이용해
    [orange] { ... }

* : 범용 선택자. 모든 html요소들을 선택한다
* { ... }
. : 클래스 선택자. 
    <a class="red"> hi </a> 일때
    .red { ... } 은 red클래스인 것들을 선택하는 선택자
# : 아이디 선택자.
    <b id="name"> JM </b> 일때
    #name { ... } 은 name이라는 id를 선택하는 선택자

    속성 선택자[]가 가장 많이 이용됨
    - 값이 있는 속성을 선택할 때 [type="next"]{...}

    사용자 행동 의사 클래스 선택자: 사용자의 행동에 따라 작동하는 것
    - 선택자 : hover
    - 선택자 : focus

    선택자 중첩으로 특정 요소만 뽑아내기 가능!

    자손 결합 선택자: 선택자 .클래스
    자식 결합 선택자: 선택자 > .클래스
    형제 선택자: 선택자 p ~ button
    인접 형제 선택자: p +

    선택자 여러개 동시 선택
    : a, b, c : hover{...}