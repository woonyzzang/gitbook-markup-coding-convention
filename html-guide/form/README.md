# form
> 폼 컨트롤 요소를 작성할 떄 form, fieldset, legend 요소를 다음과 같이 선언한다. 단, 필요에 따라 개별적으로 사용할 수 있다.

``` html
<form>
    <fieldset>
        <legend>...</legend>
        [form control element here]
    </fieldset>
</form>
```

참고: form 요소는 마크업시 기본적으로 사용 하지 않는다. 만약 form 요소를 넣어야 할 경우 action 속성은 서버 쪽 폼 핸들러이나 필수 선언 속성이므로 마크업 단계에서 선택에 따라 선언 할 수 있다.