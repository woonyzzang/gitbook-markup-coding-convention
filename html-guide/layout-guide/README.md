# Layout Guide

## HTML 4.01 ⁄ XHTML 1.0 기본 레이아웃
신규 HTML문서를 작성할 때는 다음과 같은 기본 HTML문서 구조를 따른다.

``` html
<body>
<!-- skip -->
<div id="skip">
    <a href="#">본문 바로가기</a>
    <a href="#">메뉴 바로가기</a>
</div>
<!-- //skip -->
<div id="wrap">
    <!-- header -->
    <div id="header">헤더 영역</div>
    <!-- //header -->
    <!-- container -->
    <div id="container">
        <!-- content -->
        <div id="content">콘텐츠 영역</div>
        <!-- //content -->
    </div>
    <!-- //container -->
    <!-- footer -->
    <div id="footer">푸터 영역</div>
    <!-- //footer -->
</div>
</body>
```

* 스킵네비게이션 바로가기(목차) 위치는 가장 상단에 위치시킨다.
* 레이아웃은 전체를 "wrap"으로 감싸고 "header", "container", "footer" 로 나눈다.
* h1(서비스명), h2(메인메뉴,본문,이용약관...), h3(세부컨텐츠, 핵심컨텐츠), h4(서브컨텐츠) , h5~h6(될 수 있으면 안쓴다.)

## HTML5 기본 레이아웃
HTML5 DTD를 선언할시에는 다음과 같은 구조를 따른다.

``` html
<body>
<!-- skip -->
<div id="skip">
    <a href="#">본문 바로가기</a>
    <a href="#">메뉴 바로가기</a>
</div>
<!-- //skip -->
<div id="wrap">
    <!-- header -->
    <header>헤더 영역</header>
    <!-- //header -->
    <!-- container -->
    <div id="container">
        <!-- content -->
        <main id="content">콘텐츠 영역</main>
        <!-- //content -->
    </div>
    <!-- //container -->
    <!-- footer -->
    <footer>푸터 영역</footer>
    <!-- //footer -->
</div>
</body>
```

* article : 태그 자체로 완전한 하나의 개별 컨텐츠 article은 그 안에 section을 가질 수 있다.
* section : 제목 태그(Heading Tag)를 지닌 영역 구분.