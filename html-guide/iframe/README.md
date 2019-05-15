# iframe
> iframe 요소를 사용하면 다음과 같은 문제점이 있다.

* iframe 요소를 포함하는 페이지의 도메인과 iframe 요소에서 불러오는 페이지의 도메인이 다르면 크로스 도메인 설정을 위해 별도의 소스 코드가 추가되어 성능에 영향을 줄 수 있다.
* iframe 요소의 높이값을 콘텐츠에 따라 유동적으로 지정해야 한다면 별도의 자바스크립트 코드가 추가되어 성능에 영향을 줄 수 있다.
검색 엔진에서 iframe 요소의 내용만 추출해서 표시하면 전체 페이지의 레이아웃이 비정상적으로 보일 수 있으며, 주변 맥락(머리글, 바닥글, 메뉴)이 노출되지 않아 검색 엔진 최적화(SEO) 관점에서도 적합하지 않다.
* iframe 요소는 마지막에 로드되지 때문에 페이지 로딩 초기에는 화면이 비어 보일 수 있다.
* 모바일에서는 iframe 요소의 스크롤에 대한 렌더링이 브라우저별로 다르며, CSS 말 줄임이 동작하지 않는 브라우저가 있다.

이와 같은 이유로 아이프에임은 가급적 사용하지 않도록 권장한다. 부득이하게 사용해야 할 때는 다음 규칙을 준수한다.

* src, width, height, title, frameborder, marginwidth, marginheight, scrolling 순서로 속성을 선언한다.
* 스크린리더 사용자를 위해 title 속성에 제목을 표기한다. 단 iframe 요소 윗부분의 헤딩 요소가 아이프레임의 제목 역활을 할 때는 title 속성을 생략할 수 있다.

**– HTML 경우**
``` html
<iframe src="" width="" height="" title="공지사항 게시판" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"></iframe>
```
**– HTML5 경우**
``` html
<iframe src="" width="" height="" title="공지사항 게시판" frameborder="0"></iframe>
```

HTML5 DTD 선언할 때 frameborder, marginwidth, marginheight, scrolling 속성은 사용할 수 없다.
단, frmaeborder 속성은 CSS 속성으로 제어 할 수 없으므로 허용한다.