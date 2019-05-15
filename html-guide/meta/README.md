# meta
> 문서의 기본 인코딩, 뷰포트, 스크립트 형식, 스타일 형식 순으로 요소를 선언한다. 뷰포트는 모바일 브라우저에 대응하는 HTML의 경우에만 선언한다.

* 검색 엔진 최적화를 위하여 meta 요소를 이용하여 문서 제목을 추가 명시한다.
* 컨텐츠 상세 페이지에서는 컨텐츠 제목 만을 표기한다.
* 서비스홈에서는 서비스명 만을 표기, 서브 섹션홈에서는 하위섹션명 : 서비스명 을 표기한다.
* 컨텐츠 제목의 특수기호가 들어갈시 엔티티코드로 변환가능한 기호는 반드시 escape 되어야 한다.

``` html
<meta charset="utf-8"> <!-- 필수 사항 -->
<meta http-equiv="X-UA-Compatible" content="IE=edge"> <!-- 선택 사항 -->
<meta http-equiv="Content-Style-Type" content="text/css"> <!-- 선택 사항 -->
<meta http-equiv="Content-Script-Type" content="text/javascript"> <!-- 선택 사항 -->
<meta name="viewport" content="width=device-width,initial-scale=1"> <!-- 모바일, 반응형 대응 -->
<meta name="format-detection" content="telephone=no"> <!-- 모바일, 반응형 대응 -->
<meta name="publisher" content="[Google] UI Dev Team"> <!-- 필수 사항 -->
<meta name="author" content="Joe Seung Woon"> <!-- 필수 사항 (마크업 개발자명) -->
<meta name="title" content="Google"> <!-- 선택 사항 (메인페이지) -->
<meta name="title" content="Web⁄Mobile Integration : Google"> <!-- 선택 사항 (서브페이지) -->
<meta name="description" content="Digital Agency - Google"> <!-- 권장 사항 (SEO 최적화) -->
```