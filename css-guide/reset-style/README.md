# 초기 스타일시트
> 크로스브라우징을 위해 각 태그관련 속성을 초기화 시켜주는 CSS로 PC와 Mobile에서의 환경을 고려하여 각각 초기 스타일 시트 파일을 사용한다. 각 프로젝트나 서비스 개편시 해당 문서를 활용하여 초기화시켜준다. 그리고 기능적으로 공통적으로 자주 사용되는 속성은 Global Class로 정의하여 선택적으로 사용한다.

## PC – CSS 초기 문서
``` css
@charset "utf-8";
/* <Google> UI Dev Team JSW 180628 */

/* =Reset */
html,body,div,span,object,iframe,h1,h2,h3,h4,h5,h6,p,blockquote,pre,abbr,address,cite,code,del,dfn,em,img,ins,kbd,q,samp,small,strong,sub,sup,var,b,i,dl,dt,dd,ol,ul,li,fieldset,form,label,legend,table,caption,tbody,tfoot,thead,tr,th,td,article,aside,canvas,details,figcaption,figure,footer,header,hgroup,menu,nav,section,summary,time,mark,audio,video{margin:0;padding:0}
body,h1,h2,h3,h4,h5,h6,select,input,textarea,button{font-family:Dotum,'돋움',Helvetica,'Apple SD Gothic Neo',sans-serif}
body{/*-webkit-text-size-adjust:none;*/font-size:14px;color:#222;word-break:break-all}
input,select,textarea,button{font-size:14px;vertical-align:top}
button,input,textarea{-webkit-border-radius:0;border-radius:0}
button{background-color:transparent;cursor:pointer}
article,aside,details,figcaption,figure,footer,header,hgroup,menu,nav,section{display:block}
table{table-layout:fixed;width:100%;border-collapse:collapse;border-spacing:0}
ol,ul{list-style:none}
em,address{font-style:normal}
img,fieldset,iframe{border:0}
img{max-width:100%;height:auto;vertical-align:top}
a{color:#333;text-decoration:none}
area{outline:0}
input::-ms-clear{display:none}
input[type=date]::-webkit-inner-spin-button{display:none}
input[type=number]::-webkit-inner-spin-button,
input[type=number]::-webkit-calendar-picker-indicator{display:none}
input[type=number]{-moz-appearance:textfield}
select{border-radius:0}
```

## Mobile – CSS 초기 문서
``` css
@charset "utf-8";
/* <Google> UI Dev Team JSW 180628 */

/* =Reset */
:root{font-size:10px}
body,button,dd,dl,dt,fieldset,form,h1,h2,h3,h4,h5,h6,input,legend,li,ol,p,select,table,td,textarea,th,ul{margin:0;padding:0}
body,button,h1,h2,h3,h4,h5,input,select,table,textarea{font-family:HelveticaNeue-Light,AppleSDGothicNeo-Light,sans-serif;font-size:1.5rem;line-height:1.5}
body{-webkit-text-size-adjust:none;word-break:break-all}
table{border-collapse:collapse}
img,fieldset,iframe{border:0}
img{max-width:100%;height:auto;vertical-align:top}
ol,ul{list-style:none}
address,em{font-style:normal}
a{color:inherit;text-decoration:none;-webkit-tap-highlight-color:rgba(0,0,0,.1)}
button,input,textarea{-webkit-border-radius:0;border-radius:0}
button{background-color:transparent}
select{border-radius:0}
```

## PC ⁄ Mobile – Global Class (선택적 사용)
``` css
## 스킵 네비게이션
/* =Skip Navigation */
#skip{position:relative;z-index:1000}
#skip a{position:absolute;top:-50px;left:0;padding:6px 15px;background-color:#231f20;border:1px solid #ed1c24;color:#fff}
#skip a:active,
#skip a:focus{top:0;text-decoration:none;cursor:pointer}
#skip span{display:inline-block}

## 웹킷계열 브라우저 커스텀 스크롤바
/* =Webkit Browser Custom Scrollbar */
::-webkit-scrollbar{width:8px;height:3px;border-left:0;background:rgba(0,0,0,.1)}
::-webkit-scrollbar-track{background-color:#eee}
::-webkit-scrollbar-thumb{background-color:#000;border-radius:0}

## 웹킷계열 플레이스 홀더 컬러
/* =Custom Placeholder */
::-webkit-input-placeholder{color:#888}

/* =Set Class */
.blind{overflow:hidden;position:absolute;width:1px;height:1px;clip:rect(0 0 0 0);margin:-1px;color:transparent} /* 사용된 이미지내 의미있는 텍스트의 대체텍스트를 제공할때 */
.dimmed{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1000;background-color:#000;opacity:.7;filter:alpha(opacity=70)} /* 딤드레이어 */
.eps{display:inline-block;overflow:hidden;white-space:nowrap;text-overflow:ellipsis} /* 한줄 말줄임*/
.show{display:block} /* 노출 */
.hide{display:none} /* 숨김 */
.fl{float:left} /* 좌측 플로팅 */
.fr{float:right} /* 우측 플로팅 */
.clearfix:after{display:table;content:'';clear:both} /* 플로팅 해제 */
.tbl{table-layout:fixed;display:table;width:100%} /* 테이블 */
.row{display:table-row} /* 테이블 행 */
.cell{display:table-cell;width:100%;vertical-align:top} /* 테이블 셀*/
```

참고: 각 프로젝트나 작업시 상황에 따라 CSS 초기 문서는 약간씩 변경해서 사용될 수 있다.

``` css
## 스프라이트 아이콘
/* =Icon */
[class~=ico]{display:inline-block;overflow:hidden;background-repeat:no-repeat;vertical-align:top}
.ico_{name}{width:'';height:'';background-image:url()}
```