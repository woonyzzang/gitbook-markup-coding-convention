# CSS 코드 기본 규칙
> CSS 코드를 작성할 때 다음과 같은 기본 규칙을 준수한다.

## W3C Validation
모바일에서 CSS는 사용 가능한 핵(hack)과 CSS3 속성을 제외하고는 W3C Validation을 통과해야 한다.

## CSS 로드
* CSS 데이터를 로딩할 경우 @import 방식은 사용하지 않는다. (일부 브라우저에서 이미지 로딩 후 적용되는 이슈 등이 있다.
* External 방식에서는 인코딩 선언인 charset은 반드시 표기한다.

## 인코딩
글꼴 이름이 영문이 아닐 때 브라우저에서 컨텐츠를 바르게 표시하고, HTML에서 불러온 스타일을 제대로 렌더링 하려면 반드시 CSS 인코딩을 선언해야 한다. HTML과 동일한 인코딩을 문서 첫줄에 공백 없이 선언한다.

``` css
@charset "utf-8"
```

## 영문 소문자 사용
모든 속성은 영문 소문자로만 작성한다.

[ 소문자 작성 예 ]

**잘못된 예**
``` css
.class{Font-Family:AppleGothic}
```
**올바른 예**
``` css
.class{font-family:AppleGothic}
```

## 따옴표 사용 범위
공백이 포함된 글꼴 이름, 한글 글꼴 이름, 데이터 타입, filter 속성의 파라미터 값은 작은 따옴표(")로 감싸고, @charset 을 선언할 때는 속성값을 큰 따옴표("")로 감싼다. 그 외의 경우에는 따옴표를 사용하지 않는다. filter 속성의 파라미터값에 따옴표를 사용하는 것은 선택 사항이다.

url 데이터 타입에서는 작은 따옴표를 사용하지 않는다.

[ 따옴표 사용 예 ]

**잘못된 예**
``` css
font-family:돋움
```
``` css
filter:progid:DXImageTransform.Microsoft.AlphaImageLoader(src="bg.png",sizingMethod="scale")
```
``` css
background:url('bg.gif') no-repeat
```
``` css
content:""
```
``` css
@chaset 'utf-8'
```
**올바른 예**
``` css
font-family:'돋움'
```
``` css
filter:progid:DXImageTransform.Microsoft.AlphaImageLoader(src='bg.png',sizingMethod='scale')
```
``` css
background:url(bg.gif) no-repeat
```
``` css
content:''
```
``` css
@chaset "utf-8"
```

## 마지막 세미클론 사용 지양
마지막 속성의 세미클론(;)은 삭제한다.

[ 마지막 세미클론 예 ]

**잘못된 예**
``` css
.class{font-size:12px;color:#333;}
```
**올바른 예**
``` css
.class{font-size:12px;color:#333}
```