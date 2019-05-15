# 공백
> CSS 파일의 용량이 커지지 않도록 불필요한 공백을 최소화한다.

## 선택자 간 공백 제거
쉼표로 구분되는 선택자 간 공백은 개행 한다.

[ 선택자 간 공백 개행 예 ]

**잘못된 예**
``` css
a:hover, a:active, a:focus{text-decoration:underline}
```
**올바른 예**
``` css
a:hover,
a:active,
a:focus{text-decoration:underline}
```

참고: reset 초기화 관련같은 css 선택자 간 공백은 선택적으로 예외로 할 수 있다.
단, 이런 경우에는 쉼표로 구분되는 선택자 간 공백들은 제거한다.


[ 선택자 간 공백 제거 예 ]

**잘못된 예**
``` css
a:hover, a:active, a:focus{text-decoration:underline}
```
**올바른 예**
``` css
a:hover,a:active,a:focus{text-decoration:underline}
```

## 속성 간 공백 제거
속성 간 공백 및 속성값 사이 공백은 제거한다.

**잘못된 예**
``` css
.class p{color:#333; line-height:16px}
```
``` css
.class a{font-size:13px ;background-color:#eee}
```
``` css
body{font-family:’돋움’, dotum}
```
**올바른 예**
``` css
.class p{color:#333;line-height:16px}
```
``` css
.class a{font-size:13px;background-color:#eee}
```
``` css
body{font-family:'돋움',dotum}
```

## 중괄호 좌우 공백 제거
중괄호의 좌우 공백은 제거한다.

**잘못된 예**
``` css
.class p {color:#000}
```
``` css
.class p{ color:#000; line-height:18px }
```
**올바른 예**
``` css
.class p{color:#000}
```
``` css
.class p{color:#000;line-height:18px}
```