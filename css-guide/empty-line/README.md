# 빈 줄
> 의미 있는 객체를 구분할 목적으로 코드 그룹 사이에 빈 줄을 넣을 수 있다. 단, 빈 줄은 한 줄을 넘지 않게 한다. 빈줄의 사용은 선택 사항이다.

[ 빈 줄 사용 예 ]

**잘못된 예**
``` css
<style>
/* =의미 있는 그룹1 */
.class1{border:1px solid #000}
.class1 img{vertical-align:top}
[빈 줄]
[빈 줄]
/* =의미 있는 그룹1 */
.class2{border:1px solid #000}
.class2 img{vertical-align:top}
</style>
```
**올바른 예**
``` css
<style>
/* =의미 있는 그룹1 */
.class1{border:1px solid #000}
.class1 img{vertical-align:top}
[빈 줄]
/* =의미 있는 그룹1 */
.class2{border:1px solid #000}
.class2 img{vertical-align:top}
</style>
```