# 주석
> CSS 주석은 다음과 같이 표기하며, 기본 형식에 맞게 작성한다.

## 기본 형식

``` css
/* =주석내용 */ (한글일 경우)

/* =List Type */ (영문일 경우)
```

* 주석 기호와 주석 사이에는 반드시 공백 한 칸이 있어야 한다.
* 주석 기호와 주석 내용 사이의 줄 바꿈은 허용하지 않는다. 단, 주석 내용 간 줄바꿈은 허용한다.
* 종료 주석은 사용하지 않는다.
* 주석 작성시 접두어(prifix)로 = 기호를 표기해서 작성한다.
* 주석을 영문으로 작성할때는 카멜 표기법으로 작성한다.

유지보수 시 추가 및 수정이 되어 주석을 기입하는 경우 해당 수정날짜(YYMMDD, 이름 형식)로 시작하며, 한 줄일 경우 해당 선언 마지막 뒤에 표시한다.(운영관련 시 주석처리는 = 접두어(prifix)를 사용하지 않는다.)

``` css
/* 180628 JSW - GNB 수정 */
.gnb_comm{overflow:hidden;width:978px;clear:both}
.gnb_comm li{float:left;height:38px}
.gnb_comm .menu{display:block;overflow:hidden;height:38px}
.gnb_comm .home{width:79px}
.gnb_comm .roadmap{width:98px}
.gnb_comm .on .menu{margin:0 -1px}
/* //180628 JSW - GNB 수정 */

.news .on .menu {margin:0 -1px} /* 181109 LNY 수정 */
```

주의: 마크업과 개발의 편의를 위해 작성한 주석 및 불필요한 주석은 실제 서비스를 적용할 때 반드시 삭제한다. 단, 작성자 정보는 삭제하지 않는다.

## 작성자 정보 표기

작성자 정보에는 소속 부서, 영문 이름 이니셜, CSS 파일 생성 날짜(YYMMDD 형식)를 작성하며, 유지보수만 담당하는 경우라도 모두 기입한다. 작성자 정보 및에는 빈줄을 한 둘 둬서 스타일을 선언한 문장돠 구분되게 한다.

``` css
@charset "utf-8"
/* <Google> UI Dev Team JSW 180628, LNY 181109 */

/* =Reset */
...
```

참고: 작성자 정보 주석일 경우에는 접두어(prifix) = 기호를 작성하지 않는다.

협업하는 작업자들과 동일한 날짜에 작성을 하게 된다면 생성날짜 형식을 단축시켜 뒤에다 한번에 표기 할 수 있다.

``` css
@charset "utf-8"
/* <Google> UI Dev Team JSW, LNY 180628 */

/* =Reset */
...
```

외주나 프리랜서 작업자일 경우에는 중괄호({}) 안에 영문 이름 이니셜을 표기한다.

``` css
@charset "utf-8"
/* <Google> UI Dev Team JSW 180628, {LNY} 181109 */

/* =Reset */
...
```