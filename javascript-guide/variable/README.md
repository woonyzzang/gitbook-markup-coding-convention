# 변수
> 암묵적인 전역변수는 절대로 사용하지 않지만 꼭 필요한 경우에는 허용한다. 변수 선언 부와 처리 부는 라인을 띄운다.

``` javascript
// Bad
myglobal = 'hello';
```
``` javascript
// Good
function sum(x, y) {
    var result = x + y;
    
    return result;
}

// Bad
function sum(x, y) {
    result = x + y;
    
    return result;
}
```
``` javascript
// Good
function foo() {
    var a, b;

    a = b = 0;
}

// Bad
function foo() {
    var a = b = 0; // var a = (b = 0);와 같다. b가 암묵적 전역이 된다.
}
```