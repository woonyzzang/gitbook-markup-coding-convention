# 속성 선언 순서

## 공통 선택자 사용 지양
속성은 레이아웃과 관련이 큰 것부터 선언한다. 관련 속성은 대표되는 속성 다음으로 선언하며, 다음 표에 표기된 순서대로 선언한다.

[ 속성 선언 순서 ]

| **순서** | **의미** | **대표되는 속성(그룹)** | **관련 속성** |
| --- | --- | --- | --- |
| 1 | 표시 | display | visibility |
| 2 | 넘침 | overflow | – |
| 3 | 흐름 | float | clear |
| 4 | 위치 | position | top, right, bottom, left, z-index |
| 5 | 크기 | width & height | – |
| 6 | 간격 | margin & padding (그룹) | – |
| 7 | 테두리 | border (그룹) | – |
| 8 | 배경 | background (그룹) | – |
| 9 | 글꼴 | font (그룹) | color, letter-spacing, text-align, text-decoration, text-indent, vertical-align, white-space 등 |
| 10 | 동작 | animation | animation, transform, transition, marquee 등 |
| 11 | 기타 | – | 위에 언급 되지 않은 나머지 속성, 글꼴 관련 속성 이후에 선언하며 기타 속성 내의 선언 순서는 무관함. |

**속성 선언 순서 기준**
* 1~6: 레이아웃
* 7~8: 테두리 ⁄ 배경
* 9: 글꼴
* 10: 동작
* 11: 기타

대표되는 속성 중 (그룹)으로 표기된 것은 약식 속성으로, 약식속성을 선언했을때 속성값의 순서와 동일하게 전체 속성을 선언한다. 다음 표의 선언 순서를 참고한다.

[ 약식 속성의 전체 속성 선언 순서 ]

| **약식 속성** | **전체 속성 선언 순서** |
| --- | --- |
| margin | margin-top, margin-right, margin-bottom, margin-left |
| padding | padding-top, padding-right, padding-bottom, padding-left |
| border | border-top, border-right, border-bottom, border-left, border-width, border-top-width, border-right-width, border-bottom-width, border-left-width, border-style, border-top-style, border-right-style, border-bottom-style, border-left-style, border-color, border-top-color, border-right-color, border-right-color, border-bottom-color, border-left-color, border-image, border-radius, border-collapse, border-spacing |
| background | background-color, background-image, background-repeat, background-position, background-size, background-attachment, background-origin, background-clip |
| font | font-style, font-variant, font-weight, font-size, font-family, line-height |
| animation | animation-name, animation-duration, animation-timing-function, animation-delay, animation-iteration-count, animation-direction |
| transition | transition-property, transition-duration, transition-timing-function, transition-delay |

## 속성값 축약
CSS 최적화를 위해 다음과 같이 속성값을 축약한다.

[ 속성값 축약 예 ]

| **축약 전** | **축약 후** | **설명** |
| --- | --- | --- |
| #555555 | #555 | **16진수 컬러 코드값**<br>동일한 값으로 이루어진 16진수 컬러 코드값은 세 자릿수로 축약해서 사용한다. 단, 인터넷 익스플로러 전용 속성인 CSS filter를 사용하면 축약 속성을 인식 못하는 오류가 있으므로 filter 컬러 코드값의 속성값은 축약하지 않는다.
| #ff6600 | #f60 ||
| background-position:left center | background-position:0 50% | **위치값**<br>문자로 표현한 위치값은 숫자로 변경한다. |
| top:0px | top:0 ||
| background-position:left center | background-position:0 50% | **0 단위**<br>속성값이 0이면 단위를 표시하지 않는다. |
| padding:20px 20px 20px 20px | padding:20px ||
| background-position:left center | background-position:0 50% | **동일한 속성값**<br>상, 우, 하, 좌의 속성값이 동일하면 축약한다. |
| margin:0 auto 0 auto | margin:0 auto ||
| padding:20px 30px 50px 30px | padding:20px 30px 50px ||
| border-color:#ccc #eee #ccc #eee | border-color:#ccc #eee ||

참고: 문자로 표현된 위치값을 숫자로 변환할 때 다음과 같이 한다.
* top, left: 0
* right, bottom: 100%

## 약식 속성 사용 범위
border와 background는 약식 속성을 우선적으로 사용하고, font 약식 속성은 사용하지 않는다.

**border**

속성값은 border-width, border-style, border-color 순으로 선언한다. 테두리 스타일 속성을 초기 선언할 때는 반드시 border 단일 속성을 사용하고, 이후 테두리의 부분적인 속성이 변경되면 border 관련 속성(border-width, border-style, border-color)을 선언한다.

``` css
.class{border:1px solid #ccc}
.class_v1{border-color:#666}
.class_v2{border-style:dotted}

.class2{border-top:1px solid #ccc}
.class2_v1{border-top-color:#666}
.class2_v2{border-top-style:dotted}
```

테두리의 상, 우, 하, 좌 스타일이 2개이상 다르면 공통 스타일을 약식 속성으로 선언한 후 다른 부분은 관련 속성으로 선언한다.

**background**

속성값은 background-color, background-image, background-repeat, background-position, background-size, background-attachment, background-origin, background-clip 순서로 선언한다. 배경 스타일 속성을 초기 선언할 때는 반드시 background 단일 속성을 사용하고, 이후 배경의 부분적인 속성이 변경되면 background 관련속성(background-color, background-image, background-repeat, background-position, background-size, background-attachment, background-origin, background-clip)을 선언한다.

``` css
.class{background:#ccc url(bg.gif) no-repeat}
.class_v1{backgrond-position:0 -50px}
.class_v2{backgrond-position:0 -100px}
```

[ 테두리 스타일이 2개 이상 다를 경우 약식 속성 선언의 예 ]

**잘못된 예**
``` css
.class{border:1px solid #ddd;border-bottom:1px solid #eee;border-left:1px solid #eee}
```
``` css
.class{border-top:1px solid #ddd;border-right:1px dotted #ddd;border-bottom:1px solid #eee;border-left:1px dotted #eee}
```
**올바른 예**
``` css
.class{border:1px solid;border-color:#ddd #eee #eee}
```
``` css
.class{border:1px;solid-style:solid dotted;border-color:#ddd #ddd #eee #eee}
```

**font**

글꼴 스타일 선언시 font-style > font-variant > font-weight > font-size > line-height > font-family 순서로 선언하며, 약식 속성으로 선언하지 않는다. 예를 들어 다음과 같이 약식 속성으로 선언하면 font-weight:bold는 상속되지 않고 font 속성의 기본값인 font-weight:normal로 변경되기 때문에 불필요한 속성값을 선언해야 하는 문제가 있다.

``` css
.class{font-weight:bold;font-size:12px;font-family:dotum}
.class p{font:15px gulim}
```

결국, .class p의 글꼴 스타일은 다음과 같아진다.

``` css
.class{font-family:gulim;font-style:normal;font-variant:normal;font-weight:normal;font-size:15px;line-height:normal}
```

## 한글 글꼴 선언
한글 글꼴을 선언할 때 한글이나 영문 이름 중 하나로만 표기하면 특정 브라우저에서 글꼴을 올바르게 출력하지 못하는 경우가 있으므로 반드시 한글과 영문 이름을 모두 선언한다.


[ 글꼴 선언 예 ]

**잘못된 예**
``` css
font-family:'돋움'
```
**올바른 예**
``` css
font-family:'돋움',dotum
```
``` css
font-family:dotum
```