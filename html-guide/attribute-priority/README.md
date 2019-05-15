# Attribute 우선순위
> 일관성있는 코드를 작성하기 위해 속성 선언시 정해진 우선순위의 규칙을 준수한다.

## Attribute 작성
Attribute 값은 큰 따옴표(" ")로 묶는다.

## Attribute 우선순위
Attribute의 우선 순위는 다음 순위를 따른다.

[ 요소 속성 우선순위 목록 ]

| **우선순위** | **속성** |
| --- | --- |
| 1 | rel |
| 2 | type |
| 3 | href, src |
| 4 | target |
| 5 | title |
| 6 | width, height |
| 7 | 기타 속성 |
| 8 | value, alt |
| 9 | name |
| 10 | id |
| 11 | class |
| 12 | style |

특정 요소에 class와 style을 선언할 때는 선언 순서를 제일 뒷부분에 선언한다.

``` html
<a href="" target="" title="" id="" style="">...</a>
<img src="" title="" width="" height="" alt="" id="" style="">
<input type="" title="" size="" maxlength="" name="" id="" class="" style="">
```