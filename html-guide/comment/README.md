# 주석
> HTML 주석의 시작과 종료는 다음과 같이 표기하며, 기본 형식에 맞게 작성한다.

``` text
@기본 형식
시작 주석: <!-- 주석 내용-->
종료 주석: <!-- //주석 내용 -->
```

* 주석기호와 주석 내용 사이에는 반드시 공백이 한 칸 있어야 한다.
* 주석 기호와 주석 내용 사이의 줄 바꿈은 허용하지 않는다. 단, 주석 내용 사이의 줄바꿈은 허용한다.
* 시작과 종료 주석의 주석 내용은 동일해야 한다.

[ 주석 기본 형식 예 ]

**잘못된 예**
``` html
<!--GNB-->
```
``` html
<!--* GNB *-->
```
``` html
<!-- GNB
-->
```
``` html
<!-- GNB 시작 -->
...
<!-- //GNB 끝 -->
```
**올바른 예**
``` html
<!-- GNB -->
...
<!-- //GNB -->
```

마크업과 개발의 편위를 위해 작성한 주석은 실제 서비스를 적용할 때 반드시 삭제한다.

**주의사항**
* 공통 : 너무 많은 주석은 유령문자버그를 생성하므로 되도록 자제 한다.
* HTML : 주석 시작과 종료 구분자("--") 사이에는 공백 문자(white space)가 올 수 없다.
* XHTML : 주석으로 감싼 내용 안에 "--"가 오거나, 파라미터 엔티티 참조가 인식되서는 안된다.

## 레이아웃 및 콘텐츠 영역의 주석 표기
"wrap"을 제외한 레이아웃과 독립된 컨텐츠 영역의 시작과 끝에 주석을 표기하며, 레이아웃은 id 값과 동일하게 주석을 넣는다. 독립된 콘텐츠 영역의 주석 표기는 선택 사항이다. HTML 코드와 주석은 줄을 바꿔서 작성한다.

``` html
<!-- content -->
<div id="content">
    <!-- namecard -->
    <div class="namecard">...</div>
    <!-- //namecard -->
</div>
<!-- //content -->
```

## 개발 적용과 관련된 주석 표기
개발 적용과 관련된 주석은 해당되는 영역 위에 표기하며, 종료 주석은 표기하지 않는다. 주석 앞에는 [D]라는 말머리를 사용해서 담당 개발자가 반드시 확인할 수 있게 한다. 주석이 두 줄 이상이 되더라도 주석 기호는 한 번만 표기한다.

[ 개발 적용 관련 주석 표기 예 ]

**잘못된 예**
``` html
<!-- 케이스별 클래스 변화 -->
<!-- 활성화 클래스: on
비활성화 클래스: off -->
```
``` html
<img src="@tmp_btn.gif" width="25" height="25" alt="버튼">
<!-- 숨김처리
<img src="@tmp_btn_on.gif" width="25" height="25" alt="버튼">
//숨김처리 -->
```
**올바른 예**
``` html
<!-- [D] 케이스별 클래스 변화
활성화 클래스: on
비활성화 클래스: off -->
```
``` html
<img src="@tmp_btn.gif" width="25" height="25" alt="버튼">
<!-- [D] 활성화된 버튼은 파일명에 _on추가 요망
<img src="@tmp_btn_on.gif" width="25" height="25" alt="버튼">
-->
```