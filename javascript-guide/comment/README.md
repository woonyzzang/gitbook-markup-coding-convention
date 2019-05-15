# 주석
> 주석은 코드의 이해를 돕기 위한 보조문이다. 주석에는 한 줄 주석과 여러 줄 주석 두 가지가 있다. 주석은 설명하려는 구문에 맞춰 들여쓰기한다. 문장의 끝에 주석을 작성할 경우, 한 줄 주석을 사용하며 공백을 추가한다.

``` javascript
// [한 줄 주석]

// Good
function someFunction() {
    // statement에 관한 주석
    statements

    // statement에 관한 주석
    statements
}

// Bad - 들여쓰기 없음
function someFunction() {
// statement에 관한 주석
    statements

// statement에 관한 주석
    statements
}

// Bad - 첫줄의 주석에 한 줄 띄기 있음
function someFunction() {

    // statement에 관한 주석
    statements

    // statement에 관한 주석
    statements
}

// Good
var someValue += data1 + data2 - length; // 주석 표시 전후 공백

// Bad
var someValue += data1 + data2 - length;//주석 표시 전후 공백 없음

// Bad
var someValue += data1 + data2 - length; /* 여러 줄 주석 */
```
``` javascript
// [여러 줄 주석]
// 여러 줄 주석을 작성할 때는 *의 들여쓰기를 맞춘다. 주석의 첫 줄과 마지막 줄은 비워둔다.

// Good
/*
 * '*' 표시의 정렬을 맞춘다.
 */

// Bad
/*
* '*' 표시의 정렬이 맞지 않는다.
*/

// Bad - 주석의 첫줄에 문장이 옴
/* var foo = '';
 * var bar = '';
*var quux;
 */
```
``` javascript
// [코드블럭 주석 처리]
// 한 줄 주석을 사용한다.

// Good - 한 줄 주석 사용
// var foo = '';
// var bar = '';
// var quux;

// Bad - 여러 줄 주석을 사용
/*
 * var foo = '';
 * var bar = '';
 * var quux
```