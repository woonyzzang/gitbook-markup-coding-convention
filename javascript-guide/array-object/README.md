# 배열과 객체
> 배열과 객체는 반드시 리터럴로 선언한다. 배열 복사 시 순환문을 사용하지 않는다.

``` javascript
// [배열]

// Good
var emptyArr = [];
var arr = [1, 2, 3, 4, 5];

// Bad
var emptyArr = new Array();
var arr = new Array(1, 2, 3, 4, 5);
```
``` javascript
// [객체]

// Good
var emptyObj = {};
var obj = {
    pro1: 'val1',
    pro2: 'val2'
};

// Bad - 객체 생성자 사용
var emptyObj = new Object();
var obj = new Object();

// 추가: 객체의 프로퍼티가 1개인 경우에만 한줄 정의를 허용한다.
// Good
var obj = {foo: 'a'};

// Good
var obj = {
    foo: 'a'
};

// Bad - 개행 없음
var obj = {foo: 'a', bar: 'b'}

// Bad - 콜론 이전에 공백있음
var obj = {
    foo : 'a'
}

// Bad - 프로퍼티 값에 따옴표 사용, 마지막 프로퍼티에 콤마 사용
var obj = {
    'foo': 'a',
    'bar': 'b'
}
```