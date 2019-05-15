# table
> 일반적으로 레이아웃을 표현하는데 사용하지 않고, 2차원의 격자형 데이터를 표현하는데 사용한다. 표의 요약 내용을 표기해야할 때 summary 속성을 선택적으로 사용할 수 있다.

``` html
<table summary="표 요약 정보 제공">
```

HTML5 DTD 선언시 summary 속성은 사용하지 않는다.(HTML5에서 이 속성은 폐기 되었다.)

표는 다음과 같이 배치한다.

**– HTML 경우**
``` html
<table summary="짬뽕은 자장면보다 500원 비까고 열량이 50kcal 높다">
    <caption>자장면과 짬뽕의 가격과 열량 비교</caption>
    <colgroup>
        <col width="30%">
        <col width="70%">
    </colgroup>
    <thead>
        <tr>
            <th scope="col" abbr="가격">가격(won)</th>
            <th scope="col" abbr="열량">열량(kcal)</th>
        </tr>
    </thead>
    <tfoot>
        <tr>
            <th>계</th>
            <td>6,500</td>
            <td>650</td>
        </tr>
    </tfoot>
    <tbody>
        <tr>
            <th scope="row">자장면</th>
            <td>3,000</td>
            <td>300</td>
        </tr>
        <tr>
            <th scope="row">짬뽕</th>
            <td>3,500</td>
            <td>350</td>
        </tr>
    </tbody>
</table>
```
**– HTML5 경우**
``` html
<table>
    <caption>자장면과 짬뽕의 가격과 열량 비교</caption>
    <colgroup>
        <col style="width:30%">
        <col style="width:70%">
    </colgroup>
    <thead>
        <tr>
            <th scope="col" abbr="가격">가격(won)</th>
            <th scope="col" abbr="열량">열량(kcal)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope="row">자장면</th>
            <td>3,000</td>
            <td>300</td>
        </tr>
        <tr>
            <th scope="row">짬뽕</th>
            <td>3,500</td>
            <td>350</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <th>계</th>
            <td>6,500</td>
            <td>650</td>
        </tr>
    </tfoot>
</table>
```