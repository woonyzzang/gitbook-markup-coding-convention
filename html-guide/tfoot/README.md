# tfoot
> 표 바닥글을 그룹으로 나눌 때 선언한다. 이 요소는 선택적으로 사용한다.

HTML5 DTD 선언시 tfoot 요소는 tbody 요소와 tr 요소 앞에 사용하지 않는다. (HTML4.01에서는 tbody 요소 앞에 tfoot 요소를 사용 해야 했다. HTML5가 되어 tbody 요소의 전이나 후에도 사용 가능하였지만, HTML5.1부터는 tbody 요소와 tr 요소의 앞에 쓰는 것이 금지되었다.)

**– HTML 경우**
``` html
<thead>
    ...
</thead>
<tfoot>
    <tr>
        <th>계</th>
        <td>6,500</td>
        <td>650</td>
    </tr>
</tfoot>
<tbody>
    ...
</tbody>
```
**– HTML5 경우**
``` html
<thead>
    ...
</thead>
<tbody>
    ...
</tbody>
<tfoot>
    <tr>
        <th>계</th>
        <td>6,500</td>
        <td>650</td>
    </tr>
</tfoot>
```

