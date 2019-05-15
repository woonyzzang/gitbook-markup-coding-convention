# 기본 구조
> 기본적으로 전역공간이 더럽히지 않도록 익명함수를 만들어 내부에서 캡슐화 처리한다.

``` javascript
(function(global, doc, $, _) {
    'use strict';
    
    // 코드 작성
})(window, document, jQuery, _);
```