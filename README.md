# html
20240814

### html 기본 규칙
* 태그는 화살 괄호로 구분 <>
* 태그는 소문자로만 작성
* 여는태그와 닫는태그를 정확하게 입력 <></>
* 들여쓰기 활용하여 가독성 좋게 작성

### 기본 HTML 문서 구조 자동 생성 emmet
html:5  
!

### 단축키
* 줄바꿈 alt+z 

* 라이브서버 alt+L+O 

* 글꼴 확대/축소 ctrl + 마우스 휠 

* 주석 처리하기
1. (블럭지정 후) ctrl + /
(안될때는 키보드 입력기 변경 microsoft)
2. alt+shift+A

* 들여쓰기 tab/ shift tab  

## # <br> 
* 줄넘어간 것 반영시켜줌

### 이미지태그
* <img src=""> 
src 속성
따옴표안에 폴더경로 작성
혹은 이미지 주소 복사해서 붙이기
##### alt 설명☆☆☆
* <img src="img/info_2.jpg" alt="호수">

* 상대경로
내 컴퓨터 안에 있는 파일명

* 절대경로
지정된 웹 주소

### 링크 거는 태그
* <a href="주소적기">누를것적기</a>
* a태그는 href 속성을 함께 사용

### taget 속성
* 링크에 담긴 문서를 어디서 열것인지 지정하는 속성
* target="_blank" 새탭으로 열림
* _blank 새 탭에서 열기
* _self 기본값
* <a href="#"> 임시링크

<!--  -->
### 제목태그
heading
<h1>제목태그</h1>
h2 h3 h4로 진행. 
숫자 커질수록 폰트 크기 작아짐

줄복사
줄 선택된 이후 alt + shift + ↓

본문태그 
paragraph
<p></p>
p태그 안에 h태그 넣을수있음

볼드체
bold
<b></b>

<strong>
볼드로 보이긴 하는데
컴퓨터에게 중요한 태그라고 인식시킴
상위노출 시 쓰임

기울이기
italic
<i></i>

글자 중앙 줄그어주기
<del></del>

형광펜 칠
<mark></mark>

그 외 글씨 효과
sub ins small

순서가 있는 목록 태그
ordered list
<ol>
<li></li>
</ol>
 
순서가 없는 목록 
unordered list
<ul>
	<li></li>
</ul>

정의 목록 ???
definition list
<dl>
	<dt></dt>
		<dd></dd>
</dl>

입력 양식 태그
<form>
	<input type=“”>
</form>


<label for="user_id">아이디</label>
<input id="user_id" type="text"
 placeholder="아이디을 입력해주세요">
label 걸어야 컴퓨터가 구분함

<input id="user_id" type="text"
placeholder="아이디을 입력해주세요"
maxlength="6">

reauired 필수 입력 필드
reauired size 박스 가로 사이즈
minlength 최소글자수
maxlength 최대글자수
placeholder 도움말

input type=“checkbox“
(label로 감싸주면 글만 눌러도 눌림)
<label>
<input type="checkbox" name="check1" id="check1_1">이용약관</label>

input type="radio" 동그라미버튼
<label>
<input type="radio" name="radio1" 
id="radio1_1">남성</label>
<label>
<input type="radio" name="radio1"
 id="radio1_2">여성</label>

value 
폼 요소의 초기 값을 설정
없어도 화면에 요소가 표시는 되지만,
폼이 제출될때 해당 값이 전송이 안됨

텍스트 필드에 지정 시 
사용자가 수정 할 수 있는
실제 텍스트로 입력되어 표시된다


커서 세로로 크게 하는법
(한번에 여러 줄 수정할 때)
맨위 클릭-> alt+shift+드래그

드롭다운 메뉴
<select>
            <option>1월</option>
            <option>2월</option>
            <option>3월</option>
            <option>4월</option>
        </select>
    </form>
옵션 다음 selected 넣으면 해당 문자가 제일 위로 올라옴

표  
tr 행
th 제목셀
td 일반셀

<table>
<caotion>테이블의 제목</caotion>
<tr>
<th>1제목셀(왼쪽)</th>
<td>1내용셀(오른쪽)</td>
</tr>
</table>

<table><caotion></caotion>    <tr><th></th><td></td></tr></table>

<table><thead><tr> <th> data </th></tr></thead><tbody><tr><td>data</td></tr></tbody></table>
head 태그 
외부 문서 불러오기 ,스타일 태그 등 위치

표 테두리 만들기
head 태그
 title 태그 아래 style 태그 만들어주기
<style>
table, th, td {
border: 1px solid #333;
padding: 10px;
border-collapse: collapse;}
th, td{
width: 100px;
text-aligh:center;}
</style>

CSS
border 선 
padding 선 안쪽으로 들어오는 여백
border collapse 
collapse값: 
테이블 셀의 테두리를 서로 겹쳐서 하나의 테두리로 표시합니다. 셀 사이의 간격이 없으며, 테두리가 깔끔하게 정렬됩니다.
width 가로 너비
text-aligh:center; 중앙 정렬
(블록요소 안에 있는 inline요소를 정렬)

caption
표에 대한 설명 쓰기
css로 숨길 수 있음
무조건 써야함

scope
th에 추가해서 가로인지 세로인지 입력
row 가로
col 세로 
<th scope="row">
<th scope="col">

병합
rowspan="3" 
나를 포함해서 아래로 3칸 병합

colspan 나를포함해서 옆으로 병합

*필요없어진 셀 주석처리로 지워주기

table과 form
table 태그 안에는 
form태그 들어갈 수 없음 
-> form 하위에 table

(ex) 표 안에 라디오 버튼 등이 들어가야함
<form>태그를 <table>바깥에 두고, 
테이블 내에 폼 요소들
(<input>, <select>, <textarea>, 등)을 배치하는 것이 올바른 방법입니다. 이렇게 하면 전체 표가 하나의 폼으로 묶여서 제출될 수 있습니다.

비디오
이미지와 유사 .소스(src) 필요
1.컨트롤러 필요. controls
2.반복재생 원할시. loop
3.썸네일 원할시.poster=“img/  ”
4.비디오태그 하위에 source 태그 넣어서 확장자명 다른 영상 두 개로 돌발상황 대처할수있게함
5.자동재생. autoplay muted

4번 예시
<body>
<video src="img/Wildlife.mp4" 
controls loop poster="img/logo.png">
</video>
///
<video controls loop>
<source src="img/Wildlife.mp4">
<source src="img/Wildlife.webm">
</video>
</body>

오디오
audio
비디오와 매우 유사

유튜브 퍼올 때
<>퍼가기 누르기
iframe 태그 복사

논리형 데이터 (boolean)
참ture=1 거짓false=0
따로 명시하지 않으면 자동으로 0 
명시하면 1

div
블록형식 공간 분할
줄바꿈o

span 
인라인 형식 공간 분할
줄바꿈x

블록형식 태그
div,p,heading,목록

인라인 형식 태그 
span, a, img, input, 글자형식

<h1>제목태그h1</h1>
<p>단락을 나누는p</p>
<div>공간을 분할하는 div</div>
<hr>가로선을 넣어줌 
<a href="#">링크를 거는a</a>
<span>공간을 분할하는 span</span>

모두 div 태그와 같은 기능을 수행함
header, nav, aside, section, article, footer, iframe, address ... 

nav 메뉴

11sementic.html 
웹사이트 전체적인 흐름느낌
참고참고
08도 참고
