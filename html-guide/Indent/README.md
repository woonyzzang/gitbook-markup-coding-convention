# 들여쓰기
> 코드의 가독성을 높이고 HTML 구조를 쉽게 파악하기 위하여 마크업 중첩이 깊어질때 마다 들여쓰기를 사용하며 탭 1개의 크기는 공백 4칸으로 설정한다.

마크업의 깊이가 깊어질 때마다 탭 1개만큼 들여쓰지만 다음의 경우 들여쓰지 않는다.

* `<html>` 엘리먼트 의 자식 요소인 `<head>` 엘리먼트, `<body>` 엘리먼트
* `<head>` 엘리먼트의 자식 요소
* `<body>` 엘리먼트의 자식 요소

[ 들여쓰기 사용 예 ]

**잘못된 예**
``` html
<html>
<head>
[들여쓰기]<meta …>
[들여쓰기]<title>…</title>
<head>
<body>
[들여쓰기]<div id="wrap">…</div>
</body>
<html>
```
**올바른 예**
``` html
<html>
<head>
<meta …>
<title>…</title>
<head>
<body>
<div id="wrap">…</div>
</body>
<html>
```