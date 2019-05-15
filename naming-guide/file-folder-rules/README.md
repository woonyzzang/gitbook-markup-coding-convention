# 파일 및 폴더 규칙
다음과 같은 파일 및 폴더 네이밍 규칙을 준수한다.

[ 파일 및 폴더 네이밍 규칙 ]

| **분류** | **예제** | **설명** |
| --- | --- | --- |
| Folder | [p_yymmdd_프로젝트명] | 신규 프로젝트 작업 시 사용 |
|| [s_yymmdd_서스테이닝명] | 서스테이닝 작업 시 사용 |
|| [img], [css], [js], [fonts] | image, css, javascript, webfont 폴더 사용 |
|| [@listmap], [@guide] | 리스트맵, UI가이드 폴더 사용 ('@' 특수기호 프리픽스 접두어사용) |
|| [p_yymmdd_프로젝트명] / [메뉴명] | HTML 파일의 폴더 분류가 필요한 경우 사용 |
| HTML | C084628_main.html | '페이지ID.html'로 사용하거나, '페이지ID_파일이름.html'로 사용한다.(영문만 허용) |
| HTML(페이지ID 정의서가 없는 경우) | notice_view.html | '서비스영문이름_의미_상태.html'의 순서로 사용 |
|| pop_.html | 새창팝업을 사용 |
|| ly_pop_.html | 레이어팝업을 사용 |
|| ifr_.html | iframe 파일을 사용 |
| CSS | google.css | '서비스영문이름.css'로 사용한다. |
|| common.css<br>google.css | CSS 파일의 분류가 필요한 경우 사용 |
|| - | 프로모션의 경우 internal 방식으로 head 사이에 style 사용 |

[ 이미지 폴더 네이밍 규칙 ]

| **분류** | **예제** | **설명** |
| --- | --- | --- |
| Folder | – [common]<br>– [ico]<br>– [btn]<br>– [bg]<br>– [txt]<br>– [tmp]<br>– […] | img 폴더 내에 common폴더 및 대분류별 폴더가 생성되며 그 하위에 관련 image들을 넣는다. |

## 형상관리 폴더 구조 규칙

레파지토리를 사용할 경우 다음과 같은 폴더 구조 규칙을 준수한다.

[ SVN 폴더 구조 규칙 ]

| **분류** | **분기** | **예제** | **설명** |
| --- | --- | --- | --- |
| Folder | [branch] | [p_yymmdd_프로젝트명]<br>[s_yymmdd_서스테이닝명] | 신규 프로젝트 작업 및 서스테이닝 작업 시 사용 |
|| [trunk] | - | 최신 프로젝트 작업 산출물 리소스 |

