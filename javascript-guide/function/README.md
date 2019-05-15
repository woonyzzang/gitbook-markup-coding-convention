# 함수
> 함수는 함수 선언식과 표현식을 사용하여 선언한다. 함수 표현식과 함수 생성자로 선언된 함수는 호이스팅 시 값이 할당되지 않는다. 선언 이전에 사용 시 오류가 발생하므로 함수는 사용 전에 선언해야 한다. 함수 선언문은 변수 선언문 다음에 온다. function() 뒤에 중괄호는 항상 하나의 space가 존재한다.

``` javascript
// Good(1)
function doSomething(param1, param2) {
    return param1 + param2;
}

// Good(2)
var doSomething = function(param1, param2) {
    return param1 + param2;
};

// Good(3) - 이름있는 함수 표현식
var doSomething = function doSomething(param1, param2) {
    return param1 + param2;
};

// Good(4) - IIEF
(function() {
    ...
})();

// Bad(1) - 함수 생성자 사용
var doSomething = new Function('param1', 'param2', 'return param1 + param2;');

// Bad(2) - IIEF
(function() {
    ...
}());
```