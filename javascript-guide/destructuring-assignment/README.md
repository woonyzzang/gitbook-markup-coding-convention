# 선언과 할당
> 변수는 반드시 var 키워드를 사용하여 선언한다. var를 쓰지 않으면 전역변수로 설정되며, strict mode에서는 오류로 인식한다.

``` javascript
(function() {
    'use strit';
    
    title = ''; // var 없이 선언하면 strict mode에 의해 파싱타임에 오류가 발생
    var name = '';
)();
```