# 엔티티 코드
> HTML 문서안에 예약 문자나 특수 문자 및 기호를 사용할 경우 반드시 엔티티 코드로 변환한 코드로 적용 한다.

엔티티 코드를 사용하는 이유는 웹브라우저에서 예약문자와 문서내용을 구분하지 못해 생기는 문제가 발생 될 수 있기 때문이다. 예를 들어 문서 내용에 꺽쇠 괄고(<) 가 붙어 있다면 웹브라우저는 문서를 읽어 들일 때 꺽쇠 괄호를 HTML 태그 시작 기호로 렌더링 한다. 이러한 혼동을 막으려면 꺽쇠 괄호 대신 < 를 써야 한다.

* [엔티티 코드](https://entitycode.com/)
* [엔티티코드 컨버터](https://mothereff.in/html-entities)

[ entity code 참조 ]

| **character** | **entity name** | **entity number** | **description** |
| --- | --- | --- | --- |
|   | `&nbsp;` | `&#160;` | Inserts a non-breaking blank space |
| & | `&amp;` | `&#38;` | Ampersand |
| “ | `&quot;` | `&#34;` | quotation mark |
| © | `&copy;` | `&#169;` | copyright symbol |
| ® | `&reg;` | `&#174;` | registered symbol |
| ™ | `&trade;` | `&#8482;` | trademark symbol |
| “ | `&ldquo;` | `&#8220;` | Opening Double Quotes |
| ” | `&rdquo;` | `&#8221;` | Closing Double Quotes |
| ‘ | `&lsquo;` | `&#8216;` | Opening Single Quote Mark |
| ’ | `&rsquo;` | `&#8217;` | Closing Single Quote Mark |
| « | `&laquo;` | `&#171;` | angle quotation mark (left) |
| » | `&raquo;` | `&#187;` | angle quotation mark (right) |
| ‹ | `&lsaquo;` | `&#8249;` | single left angle quotation |
| › | `&rsaquo;` | `&#8250;` | single right angle quotation |
| § | `&sect;` | `&#167;` | Section Symbol |
| ¶ | `&para;` | `&#182;` | Paragraph symbol |
| • | `&bull;` | `&#8226;` | Big List Dot |
| · | `&middot;` | `&#183;` | Medium List Dot |
| … | `&hellip;` | `&#8230;` | horizontal ellipsis |
| &#124; || `&#124;` | vertical bar |
| ¦ | `&brvbar;` | `&#166;` | broken vertical bar |
| – | `&ndash;` | `&#8211;` | en-dash |
| — | `&mdash;` | `&#8212;` | em-dash |
| ¤ | `&curren;` | `&#164;` | Generic currency symbol |
| $ || `&#36;` | dollar symbol |
| ¢ | `&cent;` | `&#162;` | Cent symbol |
| £ | `&pound;` | `&#163;` | Pound |
| ¥ | `&yen;` | `&#165;` | Yen |
| € | `&euro;` | `&#8364;` | Euro symbol |
| < | `&lt;` | `&#60;` | Less than |
| > | `&gt;` | `&#62;` | Greater than |
| ≤ | `&le;` | `&#8804;` | Less than or Equal to |
| ≥ | `&ge;` | `&#8805;` | Greater than or Equal to |
| × | `&times;` | `&#215;` | Multiplication symbol |
| ÷ | `&divide;` | `&#247;` | Division symbol |
| − | `&minus;` | `&#8722;` | Minus symbol |
| ± | `&plusmn;` | `&#177;` | Plus/minus symbol |
| ≠ | `&ne;` | `&#8800;` | Not Equal |
| ¹ | `&sup1;` | `&#185;` | Superscript 1 |
| ² | `&sup2;` | `&#178;` | Superscript 2 |
| ³ | `&sup3;` | `&#179;` | Superscript 3 |
| ½ | `&frac12;` | `&#189;` | Fraction ½ |
| ¼ | `&frac14;` | `&#188;` | Fraction ¼ |
| ¾ | `&frac34;` | `&#190;` | Fraction ¾ |
| ‰ | `&permil;` | `&#8240;` | per mille |
| ° | `&deg;` | `&#176;` | Degree symbol |
| √ | `&radic;` | `&#8730;` | square root |
| ∞ | `&infin;` | `&#8734;` | Infinity |
| ← | `&larr;` | `&#8592;` | left arrow |
| ↑ | `&uarr;` | `&#8593;` | up arrow |
| → | `&rarr;` | `&#8594;` | right arrow |
| ↓ | `&darr;` | `&#8595;` | down arrow |
| ↔ | `&harr;` | `&#8596;` | left right arrow |
| ↵ | `&crarr;` | `&#8629;` | carriage return arrow |
| ⌈ | `&lceil;` | `&#8968;` | left ceiling |
| ⌉ | `&rceil;` | `&#8969;` | right ceiling |
| ⌊ | `&lfloor;` | `&#8970;` | left floor |
| ⌋ | `&rfloor;` | `&#8971;` | right floor |
| ♠ | `&spades;` | `&#9824;` | spade |
| ♣ | `&clubs;` | `&#9827;` | club |
| ♥ | `&hearts;` | `&#9829;` | heart |
| ♦ | `&diams;` | `&#9830;` | diamond |
| ◊ | `&loz;` | `&#9674;` | lozenge |
| † | `&dagger;` | `&#8224;` | dagger |
| ‡ | `&Dagger;` | `&#8225;` | double dagger |
| ¡ | `&iexcl;` | `&#161;` | inverted exclamation mark |
| ¿ | `&iquest;` | `&#191;` | inverted question mark |
| / | `&sol;` | `&#47;` | slash |