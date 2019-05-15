# 공백
> 키워드, 연산자와 다른 코드 사이에 공백이 있어야 한다. 연산자(+, -, *, /, =, etc)의 앞뒤에는 하나의 space가 존재해야 한다.

``` javascript
// Good
var value;

if (typeof str === 'string') {
    value = (a + b);
}

// Bad
var value;

if(typeof str==='string') {
    value=(a+b);
}

// Good
var arr = [1, 2, 3, 4];

// Good
someFunction(a, b, {
    prop1: 1,
    prop2: 2,
    prop3: 3
});

// Bad - 괄호 안에 공백
if ( typeof str === 'string' )

// Bad - 괄호 안 공백, 콤마 뒤 공백 없음
var arr = [ 1,2,3,4 ];

// Bad - 객체의 닫는 괄호 다음에 개행
someFunction(a, b, {
        prop1: 1,
        prop2: 2,
        prop3: 3
    }
);

```