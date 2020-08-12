# newKokoaClone2020

리뉴얼 된 newKokoaClone2020강의

## document

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
