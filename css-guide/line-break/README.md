# 줄 바꿈
> 선택자와 속성, 속성값 사이 줄 바꿈은 허용하지 않는다.

[ 줄 바꿈 사용 예 ]

**잘못된 예**
``` css
<style>
.class,
.class2,
.class3{
width:100px;
color:#999;
letter-sapcing:-1px
}
</style>
```
**올바른 예**
``` css
<style>
.class,
.class2,
.class3{width:100px;color:#999;letter-sapcing:-1px}
</style>
```