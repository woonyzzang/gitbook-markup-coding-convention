# 명명규칙
> 항상 모든 코드에 대해 아래의 동일한 명명 규칙을 사용한다.

* 공백을 허용하지 않는다.
* 예약어를 사용하지 않는다.
* 대문자 약어는 대문자 그대로 사용한다.
* 상수는 대문자와 _를 사용한다.
    * 변수, 함수는 소문자 카멜표기법을 사용한다.
    * 배열은 복수형 이름을 사용
    * 정규표현식은 'r'로 시작
    * 이벤트 핸들러는 'on'으로 시작
    * 반환 값이 불린인 함수는 'is'로 시작
    * private은 _로 시작
* 생성자는 대문자 카멜표기법을 사용한다.
* 커스텀 객체의 프로퍼티 이름에도 동일

``` javascript
// [상수]

SYMBOLIC_CONSTANTS;
```
``` javascript
// [변수]

// 숫자, 문자, 불린
dog;
variableName;

// 배열
dogs;

// 정규표현식
rDesc;
```
``` javascript
// [함수]

// 함수
getPropertyName;

// 이벤트 핸들러
onClick;
onKeyDown;

// 불린 반환 함수
isAvailable;
```
``` javascript
// [private]

_privateVariableName;
_privateFunctionName;
```
``` javascript
// [생성자]

ConstructorName;
```
``` javascript
// [커스텀 객체와 프로퍼티]

customObjectName;
customObjectName.propertyName;
customObjectName._privatePropertyName;
_privateCustomObjectName;
_privateCustomObjectName._privatePropertyName; // Bad
```
``` javascript
// [대문자 약어]

parseHTML
parseXML
```