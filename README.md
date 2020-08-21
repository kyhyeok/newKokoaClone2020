# newKokoaClone2020

리뉴얼 된 newKokoaClone2020강의

## document HTML

- html은 항상 <!DOCTYPE html>로 시작해야 한다.
- 이 행위를 하는 이유는 브라우저에세 text파일이 아닌 html 문서라고 알려주는 행위이다.
- <html></html> html태그 사이에 넣는게 html코드가 된다.
- <html lang="en"></html> html태그 안에 lang을 넣는 이유는 검색엔진들에 도움을 주기 위해서다.
- 만든 사이트의 주된 언어가 무엇인지 설정해 주는 것이다.
- 웹사이트는 head와 body 두개로 구성되어 있다.
- head에는 웹사이트의 환경을 설정할 수 있거 body는 사용자가 볼 수 있는 content를 보여준다.

# head

- 여기에 모든 행위는 <head></head> head태그안에 넣어여 한다.
- head 태그에 속해 있는 모든 태그들은 보여지지 않는다.
- title태그안에 title을 입력하면 브라우저 tab에 이름이 title로 바뀐다.
- title 태그에 있는 내용이 검색엔진에 노출이 된다.
- meta 태그의 meta는 부가적인 정보라는 뜻이고 content와 name이라는 두 개의 attribute를 가지고 있다.
- <meta content="설명" name="description" /> 검색엔진에서 보여지는 description이다.
- <meta content="키워드1, 키워드2, 키워드3" name="keywords" /> 웹사이트의 내용을 간결하고 간결하게 기술하며, 따라서 검색 엔진에 대한 웹사이트의 콘텐츠에 대한 중요한 지표다.
- <meta charset="utf-8"> charset은 브라우저에게 text를 어떻게 그려달라는지 말해준다.
- rel은 relationship의 줄인 말
- link 태그에 rel="shortcut icon"을 하면 브라우즈 tab에 아이콘이 노출 된다.
- meta 태그에 property="og:" content="" 는 카카오톡 채팅방에서 쓰이는 형식이다.

# tags

- tag는 굉장히 많아서 전부 외우는 것은 불가능에 가깝다.

# body

- 브라우저 화면상에 보여지는 모든 내용들은 body태그에 있어야 한다.

# Semantic HTML

- 문서롤 보기만해도 그 의미르 짐작할 수 있는 걸 semantic이라고 하고 html에서는 tag의 이름만 가지고도 어떤 의도로 코딩을 했는지 예상이 되는 것을 뜻한다.
- header 태그는 웹사이트의 머릿말 이라는 것을 알 수 있고 footer 태그는 꼬릿말 이라는 것을 알 수 있다.

# Non Semantic HTML

- 의미가 없는 tag들이다.
- attribute는 항상 "" 큰 따옴표로 사용해야한다.

## document CSS

- HTML이 뼈대면 CSS은 살을 붙이는 과정이다.(CSS를 잘 다루면 살이 아니라 멋짐 근육을 붙이는??)
- HTML과 CSS는 따루 두고 작업하는 것이 정석이고 HTML에 CSS를 추가하는 방법은 inline, internal, External 이렇게 세가지 방법이 있다.
- internal style은 head태그 안에 style태그를 추가해서 사용하는 방법이다.
- External style은 css파일을 include해서 외부 css파일을 사용하는 방법이다. 이때는 link 태그를 이용해서 include한다.
- inline style 각각의 tag안에 css를 추가해서 사용하는 방법으로 유지보수 할때 손이 많이 가고 코딩이 지저분해 보이기 때문에 많이 권유하는 방식은 아니다.
- 적용되는 영향력의 순서(??)는 inline > internal > External로 External에서 css를 A를 적용하고 inline에서 css B를 적용하면 화면에는 B가 적용된 모습으로 보일 것이다.
- 이 이유는 link를 통해 External style이 맨 위에 있고 그 다음 head 태그 안에 style 태그(internal)가 있고 마지막으로 태그와 안에 style(inline)가 있으면 CSS는 위에서 아래로 코드를 읽기 때문에 가장 마지막에 오는 inline style이 적용이 되어서 출력이 된다.
- 즉 코드의 순서가 가장 크게 영향을 미친다.

## CSS 규칙

- CSS Selector로 대상을 가리키고 원하는 속성을 추가하기 위해서는 중괄호 안에 코드를 작성한다.

## Cascading??

- 카스캐이딩은 목포라는 의미가 있는데 Cascading Style Sheet는 위에서부터 아래로 코딩을 읽어나가는 절차식이다.

## CSS Detail

1. Blocks and Inlines

- Blocks 옆에 아무 것도 오게 하지 허락하지 않지만 Inlines 바로 옆에 어떤 것이 와도 상관없도록 허락한다.
- Inline은 width와 height를 가질 수 없다. 애초레 너비와 높이가 없어서 width와 height속성이 적용이 안 된다.
-

2. margin

- margin은 box border의 바깥에 있는 공간이다.
- Collapsible margins은 박스가 몇 개 이든지 상관없이 margin의 경계가 같다면 하나로 취급하는 현상으로 위나 아래쪽에서만 일어난다.

3. padding

- padding은 box border의 안쪽에 있는 공간이다.

4. inline

- inline Block은 padding은 전부 적용되고 margin은 좌우면 적용이 되는데 그 이유는 inline은 높이와 너비가 없어서 위, 아래의 margin을 가질 수 없다.(무슨 이론인지는 모르겠으나 inline은 margin이 좌우로만 적용된다고 외우자)

5. display:inline Block

- inline Block에 앞서 display: block는 span같은 inline 태그에 box기능을 부여해준다.
- inline Block은 span같은 box의 형태를 가지지 않는 태그에 box의 기능을 부여해 주며 한 줄로 노출시켜 주는 기능이다.
- inline-block는 몇 가지 단점이 있는데 뭔지는 모르겠지만 default값을 가지고 있어서 공간이 생기고 정해진 형식이 없다는 것과 반응형 디자인을 지원하지 않는다.

6. display:flexbox

- 우선 flexbox를 박스를 배열해준다.
- 기본 규칙은 자식 엘리먼트에는 어떤 것도 적지 말아야 된다. 부모 엘리먼트에만 작성해야 한다. 부모 엘리먼트가 자식 엘리먼트를 제어하는 방식이다.
- flexbox에서 기본 주측은 수평이고 교차측은 수직이다. justify-content는 주측이고 align-items는 교차측인데 이 주측과 교차측은 flex-direction을 어떻게 주냐에 따라 충분히 달라질 수 있다.
- flexbox를 적용하는 순간 그 요소들은 기본값으로 nowrap(모든 요소를 같은 줄에 있게 만들어주는)이 된다.
- width값을 정했지만 그 정한값을 무시하고 화면이 작아지면 그 화면에 맞춰서 width이 작아진다.
- 이게 싫다면 flex-wrap에 wrap을 적용하면 명시한 width사이즈로 반영이 된다.(화면이 작으면 줄 바꿈을 해서라도)

6. position: fixed

- fixed는 박스가 계속 같은 자리에 머물도록 해주는 기능이다.

7. position: relative and absolute

- position의 기본 값은 static이다. static은 layout이 박스를 처음 위치하는 곳에 두는 것을 말한다.
- relative는 element가 처음 위치한 곳을 기준으로 수정하는 것이다.
- absolute는 가강 가까운 relative 부모를 기준으로 이동시켜 준다. 이때 부모 element는 position이 relative여야 한다.
- 부모 element의 position이 relative가 아닐 경우네는 body를 기준가 기준이 된다.

8. Pseudo Selecotr

- https://developer.mozilla.org/ko/docs/Web/CSS/Pseudo-classes

9. States

- Pseudo Selecotr(의사 클래스)중에서 active, hover, focus, visited, focus-within과 같은 것들을 말한다.
- active는 마우스가 대상을 클릭하고 누른 상태를 active라고 한다.
- hover은 마우스가 대상 위에 있을 때를 말한다.
- focus는 키보드로 선택되었을 때를 말한다.(input type="text")를 태그를 클릭 했을 때 깜빡이는 부분이 focus이다.
- visited는 링크에만 적용이 된다. 링크(a 태그)는 파란색에 밑줄이 기본값이다. visited는 링크가 링크를 통해 방문을 했을 경우에 적용된다.
- focus-within은 focused인 자식을 가진 부모 element이다.
- form:hover input은 마우스가 form 태그 위에 있을때 input이 적용하는 것이고 form: hover input:focus는 마우스가 form 태그 위에 있고 input이 focus가 되었을 때 적용이 된다.

10. Color

- css에서 color는 3가지 정의 방법이 있다.
- hexadecimal color(16진수 컬러) ex) #E74C3C
- RGB 방식 ex) rgb(231, 76, 60)
- RGBA 에서 A는 알파를 말하는데 투명도를 나타낸다. ex) rgba(231, 76, 60, .4) 위에 a는 css의 opacity로 투명도를 나타낸다.

11. Variables

- 원래는 custom property라고 불리운다.
- :root {요 안에 css에서 사용할 변수를 저장할 수 있다.}
- : root {--main-color: red;} h1{color:var(--main-color)} 이런식으로 사용 가능하다

12. 기타등등

- input::placeholder는 input placeholder="여기" 에서 여기 부분의 css적용을 해준다.
- ::selection은 마우스 드래그를 했을 때 css적용을 해준다.
- ::first-letter은 첫 글짜만 css적용을 해준다.
- ::first-line은 첫 줄만 css적용을 해준다.

# ADVANCED CSS

1. Transitions

- Transition은 어떤 상태에서 다른 상태로의 변화를 애니메이션으로 만드는 방법이다.
- Transition은 어떤 것을 변화하게 만들 것인지 작성하고 이 다음엔 얼마 동안 변화가 일어나게 할지 정해며 마지막에는 ease-in function을 추가한다.. 또한 ,를 사용해서 다른 부분도 추가할 수 있다.
- 하지만 여러개의 Transition을 적용할 때는 all 이라는 것을 사용하는게 편하다.
- Transition은 root element에 있어야 한다 state element에 있으면 안된다.
- stae element에 설정한 css를 root 에서 Transition을 적용하면 된다.
- ease-in function이란 Transition 마지막에 추가하는 property인 데 기본적으로 ease, linear, ease-in, easse-in-out, ease-out
- linear은 똑같이 적용이 되는것, ease-in은 처음에만 느리게 적용하는 것, ease-out은 마지막에만 느리게 적용되는 것, ease-in-out은 처음과 마지막에 느리게 적용하는 것이다.

2. Transformations

- transform이다.
- 3d로 변형시켜주는 기능이 있다.
- Transformation은 box element를 변형시키지 않는다.
- margin-right를 하면 형제 element도 움직이는데 transform : translateX(100px)하면 해당 element만 오른쪽으로 100ox 움직인다.

3. Animations

- Animation을 만들기 위해서는 규칙이 있다
- @keyframes Animation명 {이 안에서 코딩을 해야 한다.}

# Media Queries

- media query는 오직 CSS만을 이용해서 스크린의 사이즈를 알 수 있는 방법이다.
- max-width :최대 너비, min-width: 최서 너비, orientation: landscape : 핸드폰 가로일 때 orientation: portrait : 핸드폰 새로일 때
- media screen and (max-width:600px) {} => 화면이 600px보다 작으면
- media screen and (min-width:600px) {} => 화면이 600px보다 크면
- media screen and (min-width:600px) and (max-width: 700px){} => 화면이 600px보다 크고 700px보다 작으면
- media screen and (min-width:600px) and (max-width: 700px) and (orientation: landscape;){} => 가로화면 이면(모바일이나 pad종류는 가로모드가 있으니까)
- @media screen and (orientation: landscape) 가로화면 이면

# GIT AND GITHUB

1. git

- git은 파일을 계속 추적하는 것이고 파일을 이진수로 다룬다.
- 코드가 길면 파일의 히스토리를 알고 있어야 된다. 파일이 작업중 일어나는 변경 내역 등을 알고 있어야 하는데 이 때 git이 유용하다.
- git은 추적하면서 변경내역을 관리해주고 github는 그 변경내역을 업로드 한다.

2. github

- https://guides.github.com/features/mastering-markdown/
- github는 저장소(repository)가 있다. 저장소는 개발자가 작성한 코드가 살고 있는 곳이다.
- 코드를 넣은 폴더인데 코드의 변경내역과 히스토리를 갖고 있는 폴더(저장소)이다.
- commit은 기본적으로 시점이다. 이 파일에 이 버전을 저장하고 싶은 시점이다. commit은 항상 제목이 필요하다.
- github repository를 생성할 때는 소문자 + 띄어쓰기가 없이 하는것이 제일 좋다.
- vsc와 github desktop으로 만든 폴더는 같은 이름의 폴더여야 한다.
- README.md의 md는 markdown이고 REAMDE는 github repository에 항상 있어야 한다.

# CLONING TIME

1. BEM

- https://css-tricks.com/bem-101/
- Block Element Modifier라고 불린다. 사용하면 있어 보인다.

2. border Box

- css box의 width 200px 이 있다고 가정하고 padding-left 50px을 가하면 box의 width 250px이 된다.
- 그 이유는 width을 200px 설정했기 때문에 200ox을 유지하려고 하기 때문이다.
- 나는 200px을 원했지만 padding으로 인해 내가 원했던 box 크기 크게 적용이 된다. width + padding
- 이 때 box-sizing: border-box를 하면 padding을 줘도 신경쓰지 말고 box 크기를 늘리지 말라고 적용하는 것이다.

3. css

- justify-content space-between은 다른 자식 element들이 width을 가지고 있으면 원하는 위치가 있지 않을 수 있다.
- 검색엔진 구글도 검색할 때 navigation을 찾아서 ul의 li안에 있는 link를 가져오게끔 설정이 되어 있다.
