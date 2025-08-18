#HTML
### 250804 HTML시작
* 비주얼 스튜디오 코드 설치, GITHUB 회원가입, GIT 설치
* 비주얼 스튜디오 환경설정 및 Plug-in 설치
### Watch out!
git config --global user.email "you@example.com"
git config --global user.name "Your Name"

### 파일명, 폴더명 규칙
1. 영문 대소문자 사용하기(소문자 권장) 예) subTitle, sub_title
2. 숫자는 영문 뒤로 배치하기 예) sub1, main002
3. 공백 + 한글 사용금지
4. 특수문자 사용금지(#,$,%,^,&,*,(,+,\,~,★ 등..) *언더바(`_`) 하이픈(`-`) 가능
5. 이름은 의미있게 사용하기 예) images, fonts, mail, cafe 등..
6. 비주얼 스튜디오코드 실행 시 작업 폴더 연결되어있는지 확인하기
(위) 작업폴더 연결이 되지 않을경우 -> FILE -> Close Folder 후 다시 File -> Open Folder

### GIT(깃) 설치 확인
* VScode에서 단축키 'Ctrl+J' 햤를 눌러 터미널 실행 할 것
* 'git -v' GIT 설치 버전 확인 (버전결과가 나온다면 설치 되어있는 것)

### 터미널 "Ctrl + J' 기본 설정
* 윈도우 기본 터미널 powershell을 git bash로 변경
* (위 gitBash는 Git 설치 후 사용 가능)

## git 설정과 git HUB 업로드 순서 (터미널 입력 기준)
1. 'git config --list' / 현재 GIT 설정 정보 확인
2. 새 입력창이 뜨지 않을 때, 터미널에서 'ctrl + C' 또는 'Q'를 사용하여 종료 / Terminal에서는 복사의 단축키가 아닌 Cancel의 의미햣이므로 헷갈리지 말것
3. 이메일과 이름은 gitHub 가입이메일, 아이디와 일치하게 작성하는 것을 권장!
4. 위 1번에서 깃 설정정보에 name, emil이 내 정보가 아닐 때
'git config --global user.email "you@example.com"'
'git config --global user.name tsuroki (메일 아이디와 동일)'
5. 'git config --list' 사용하여 올바르게 설정됐는지 확인
6. 'git init' 현재 폴더를 작업 디렉터리 폴더로 연결, 폴더경로 옆에 **master** 확인
7. 'git branch -M main' / branch는 git directory 명칭으로, 이름을 지정해줘야 헷갈릴 일이 없으므로 이름 설정을 해주는 명령어가 'git branch -M "name"' 인 것. 여기서는 이름을 "main"이라고 설정하자고 명령어를 부여해주는 것이다.
---
8. 'git add . ' 여기서 .을 입력한 이유는 작업 수정한 모든 파일을 대기소(Stage)에 모든 파일을 업로드 하는것을 말한다. 'git add README.md'라고 작성하면 해당 파일만 업로드 하는 것.
9. 'git status' 현재 상태 또는 스테이지 확인 명령
10. 'git commit -m "기록메세지"' 현재 올리는 파일이 어떤 내용인지 기록
11. 'git remote add origin 깃허브저장주소' 깃허브 저장소 업로드 위치를 연결 시켜줌
12. 'git push origin main' 10번에서 커밋한 파일을 11번 저장소에 최종 업로드하는 명령

### 한번만 작성하면 끝인 깃 명령어
* 'git config' 이름, 이메일 설정
* 'git init' 저장소 설정
* 'git branch -M main' 저장소이름 설정
* 'git remote add origin' 저장소 주소 설정

### 작업 시 깃허브 업로드를 위해 반복해야하는 깃 명령어
* 'git add .' 
* 'git commit -m "기록메세지"
* 'git push origin main'
* 필요시 중간 점검용으로 ' git log' 또는 'git status'


# git 파일 버전 관리를 위한 명령어 
##git config --global user.email "tsuroki0210@gmail.com"
##git config --global user.name "tsuroki"

##git init
##git branch -M main
##git add .
##git commit -m ‘메세지기록’
##git remote add origin 깃허브저장소주소
##git push origin main

#HTML 작성법
*'<시작태그 속성 ="값", 속성="값"></닫기태그>
*시작태그부터 닫기태그까지 한번에 **요소**라는 명칭으로 부른다.
*속성은 시작태그에만 쓰고 닫기태그에는 속성을 쓰지 않는다.
*"파일명.html" 파일 저장시 (영문, 영어 대문자, 소문자, 숫자)으로만 작성
*HTML 장성의 시작은 항상 **구조태그**로 시작한다.

*ctrl + \ 분할 창 생성 횡
*ctrl + K + \ 분할 창 세로 생성
*ctrl + 들여쓰기, 내어쓰기
*alt + 방향키 위, 아래 

## vscode 자주쓰는 단축키
'ctrl + \ 화면 분할'
'ctrl + k, \ 화면 상 하 분할'
'Alt+Z 자동 줄 바꿈
'Alt + 상하 방향키 줄 이동'
'Shift + alt + 상하방향키 "줄 복제"'
'Shift + alt + A 주석 생성'

## 250805 자주쓰는 HTML 문서 기본태그
1. '<h1>~<h6> BLOCK TAG 1대제목~6소제목
2. '<p> block tag 제목 아래 작성하는 내용 태그
3. '<br> Inline tag 내용안에 작성하는 줄바꿈 태그
4. '<em><strong>' inline - 내용 안 강조태그
5. '<del>' inline - 쇼핑몰 원가 등에 사용하는 삭제 태그
6. '<address>' block - 회사주소 등 자회사 정보 표기에 사용하는 태그. 협력업체는 표시 X
7. '&--;' 특수문자 inline 태그. 표기하고 싶은 특수문자가 있을경우 &와; 사이에 표기

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8"><!-- 다국어 살장 -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- meta:desc, metqa:kw / 사이트 요약 ㅅ정보와 키워드 설정은 별도 -->
    <meta name="description" content="">
    <meta name="keywords" content="">
    <title>HTML|2일차 기초</title>
</head>
<body>
    
</body>
</html>

여기서 Head의 형제는 body이다.

## 레이아웃 태그
1. 그룹 DIV
2개 이상의 인라인 or 블록 요소를 묶어주는 그룹태그
2. 인라인 SPAN
2개 이상의 인라인 요소를 묶을 때 사용

## 태그 + 이름 속성
1. .class : 반복유형 분류시 사용, 반복 지정 가능
2. #id : 전체 페이지 중 단 하나의 요소에만 지정 시 사용.
** CLASS와 ID는 태그 관계없이 모든 태그에 적용할 수 있다. (태그 구분 목적)
3. class와 id는 중요한 기능일수록 부여율이 높다

## 250806 layout tag tip
1. '<div>' : 2개 이상의 블록 또는 인라인을 묶어주는 그룹,
작성과 동시에 반드시 **class 또는 id**를 의미에 맞게 부여해줄것.
2. '<div id=" "> : 반복되지 않는 고유한 이름을 설정하고 큰 틀을 작성하는데 주로 사용한다.
3. '<div class=" "> : class는 반복될 수 있는 이름을 설정하고 바깥쪽부터 안쪽까지 다양한 레이아웃에 사용.
4. '<span></span> : 2개 이상의 인라인 요소를 묶어주는 그룹. **디자인 그분을 위해 태그를 나눠야 할 때, 형제관계를 띄는 태그가 인라인 요소일 경우** 의미가 없는 부분에 자주 이용.
5. 'class or id' : 클래스와 아이디 속성은 구분이 필요한 모든 태그에 추갸로 작성할 수 있다. **태그가 2개 이상 연속적으로 작성되어 구분이 필요한  경우** 클래스를 주로 사용한다.
6. '<a>' 다른 페이지나 같은 페이지의 어느 위치, 파일, 이메일 주소와 그 외 다른 URL로 연결하는 하이퍼 링크.
7. '<a href=" ">' 하이퍼링크 삽입을 위한 태그 작성
8. '<a href=" " target=" "> 링크 위치 속성
_blank: 새 창에 특정 경로를 입력하여 이동시킵니다.
9. '<a href=" " target="./"> 지정된 타겟의 파일로 링크시켜, 상대경로를 지정해 파일을 열게한다.
10. '<a href=" " target="../"> 현재 지정된 경로의 상위경로로 이동한다.

## 250811 바로가기 링크 준비
* 준비 대상) 클릭할 a 요소와 이동할 위치 요소 (아이디 선언)
1. 이동할 위치에 중복되지 않는 명칭으로 아이디 설정
* ' <태그 id="review_pst"></태그>
2. 위치로 이동하는 클릭 요소에 위 1번 아이디를 이용한 링크 설정
* ' <a href ="#review_pst"> 클릭글자 또는 이미지</a>
'#이름' == 임시링크 (x) 아이디 (O)
'#' == 임시링크(O) 아이디 (x)
### 바로가기 링크 다양한 사용 예
* 같은 페이지의 다른 위치로 이동 시
* '<a href="#위치 아이디명">클릭요소</a>
* 다른 페이지의 특정 위치로 이동 시
* '<a href="#./상대경로#위치 아이디명>클릭요소</a>'
* '<a href="#./상대경로#위치 아이디명>클릭요소</a>'

## git 버전 관리
### github 폴더 복제 방법
* 'git clone 주소붙여넣기'
### 폴더 이동 방법
* cd (폴더명)
### git hub  수정된 작업물 내려받기
* git pull origin main

* clone을 통해 동일한 버전의 저장소를 내려받고 push and pull 시스템의 명령어를 이용해 파일을 Push->저장소->pull 하여 파일 관리를 진행
* 파일 관리를 통해  /집<-(main)->학원/ 집에서 push(밀기)를 하였다면 학원에서 pull(당기기)하고, 학원에서 push(밀기)를 하였다면 다시 집에서 pull(당기기) 하고

# 250813
##CSS에 대해

# CSS(CASCADING STYLE SHEETS)란

html이 뼈대, java script가 근육이라면, css는 피부 조직 및 외형을 말한다.
사용자에게 시각적으로 보이는 문서를 꾸미는 언어이며
Cascading(폭포), 단계별로 적용하는 것이 규칙이다.
부모태그부터 시작해서 자식 자손으로 이어져 가야한다.

# CSS 적용

CSS는 html과 같이 쓰느냐, 별개의 파일을 만드느냐로 나뉜다.
## CSS selector
### 선택자 {속성:값;}
* 선택자 : CSS로 디자인하는 대상
* {} : 속성과 값을 묶어주는 CSS 디자인 괄호
* 속성 : 선택자에 적용하는 속성
* 값 : 속성 값
* ; : 앞 속성값이 여기서 종료 되었다는 것을 의미.

기존, 우리가 html은 ' <태그 속성="값" 속성 "값></태그> ' 로 끝났다
그러나 CSS는 선택자 {속성=값;} 형태로 끝난다.

---

색상을 적용한다고 해보자.
/callout color
background-color

Css Tag
'<h1>제목</h1>'
일 경우

h1{color="ffffff"}
태그가 반복될 경우, 수정이 많이 어려워 지기 때문에
<h1 id="heading">제목</b1>
<h1 class="heading">제목</b1>
h1 {color: red:}
#heading{color: red;}
h1#heading{color: red;}
h1.heading{colo: red;}

이렇게 #을 통해 ID, .을 통해 CLASS를 지정하여 속성을 적용시킨다.

여기서 선택자에 코드 없이, .이냐 #만을 넣고 속성과 값을 적용시킨다면
태그와 관계없이 .이나 #을 가진 태그라면 모두 적용시키기 때문에
정확성을 높이려면 tag#id{color: red;} or tag.class{color: red;}처럼 써야한다.

그리고 선택자 끼리, tag # id와 같이 띄어쓰기를 할 경우 다른 값이 되어버리므로 공백없이 작성할 것.

## 자식에게 속성과 값을 적용할 경우
<div>
    <a>menu</a>
</div>
div a{color: red;} div의 자식부터 자손까지 전부, a를 가졌다면 color red를 부여한다
div > a{color: red;} div의 자식 중에서 a를 가진 애만 color red를 부여한다.

자식도 자손도 디자인 상관없이 색이 같아야 한다면 첫번째 방법을,
자식과 자손을 구분하여 작성하고 싶다면 두번째 방법을 사용한다.

.parent a{color: red;} 1)태그에 상관없이 / 2).parent란 class를 가졌고 / 3)a 태그의 자식과 자손을 가졌다면/ 4) color: red를 적용시켜라.

.parent > a {color: red;} 1)태그에 상관없이 / 2).parent란 class를 가졌고 / 3)a 태그의 자식이 있다면/ 4) 자식에게만 color: red를 적용시켜라.

div.parent a {color: red;} 1) div태그 중 / 2).parent란 class를 가졌고 / 3)a 태그의 자식과 자손을 가졌다면/ 4) color: red를 적용시켜라.

div.parent > a {color: red;} 1)div 태그 중 / 2).parent란 class를 가졌고 / 3)a 태그의 자식이 있다면/ 4) 자식에게만 color: red를 적용시켜라.

구별 잘 할것.

자식에 자식을 타고 들어간다면
선택자 > 선택자 > 선택자 > 선택자 ... {속성:값;} 이렇게 작성 해야 할것

---

.parent p {color: red}
.parent h1+p{color:pink;} <!-- h1+p : h1과 인접한 형제들(바로 옆) 태그에 pink를 부여 -->
.parent h1~p{color:yellow;} <!-- h1부터 그 다음 P까지 color=yellow를 부여 -->

    <div class="parent">
        <p>1</p>
        <h1>w</h1>
        <p>2</p>
        <p>3</p>
    </div>

h1~p -> h1 그 이후에 p태그를 가지고 있다면 속성값을 부여
+p -> 인접한 p에게 속성값을 부여

---

# CSS
## 캐스케이딩 스타일 시트(폭포 단계별로 작성 CSS)
### CSS 기초작성 순서
1. 'styles.reset.css' 파일 만들기
2. html파일 head안 'link:css' 사용하여 자동완성 작성하고 위 1번파일 연결
3. (html 작성 완료 기준) 부모-> 자식 순서대로 모든 선택자 작성하기 '{}' 중괄호는 비운상태로.
4. 모든 선택자 작성후 '{속성:값;}' 추가로 작성하며 디자인 진행

# 표 만들기 (HTML)
* table 태그는 모두 block특징을 가지고 있다.
* 테이블의 기본 테두리값은 0이므로 CSS진행 전 1px 설정을 권장합니다.

## tr(table row)행 , td(table data) 열 / 250814
* td(열)은 항상 tr(행) 안에 존재해야한다. tr>td
* table은 행,열을 자식, 자손으로 가지는 부모로써 존재한다.

## CSS 글자속성
### 'font-family'
* font-family : 대표글꼴, 후보글꼴, 글꼴 유형
* 글꼴 유형 : sans-serif, serif
* 그꼴명에 한글, 특수문자, 공백이 있을 경우 ' ' 따옴표 묶기
* 윈도우 기본 설치 글꼴 : 굴림, 고딕, 바탕, 궁서
* **대표글꼴이 설치가 필요한 글꼴일 경우 파일을 웹 주소로 연결해서 누구나 볼 수 있게 설정한다.**
* '<link rel="stylesheet" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.9/dist/web/static/pretendard-dynamic-subset.min.css" />'

### 'font-size'
<!-- font-size : 16px / font-size: 100% / font-size : 1.0em; -->
* 'font-size : 값확장자;'
*desktop 환경의 글자내용 크기 - 16px
*mobile / tablet 환경의 글자 내용 크기 - 14px
px단위는 절대 크기값으로 사용자 별 글자크기를 지원하지 않는다.
-> px단위가 아닌 em,rem, % 상대적 단위를 사용해야 한다.

## em, rem은 부모값을 어떻게 처리하느냐에 차이가 있다.

부모재산 10000원 자식(em)재산 5000원 -> 자식의 총 재산 10000원
부모재산 10000원 자식(rem)재산 5000원 -> 자식의 총 재산 5000원

---

부모크기 20em > 자식크기 1.5em
자식 최종 크기 > 30rem

부모크기 20rem > 자식크기 1.5rem
자식 최종 크기 1.5rem

rem 단위는 부모 상관없이 나만의 크기를 인식한다.
r(root)em이기 때문에, 자기 자신을 기준으로 삼는다.
그렇기 때문에 rem이 사용하기 편하다.

---
## 정리
* 16px 평균값 기준으로 피그마, 포토샵 등에서 디자인한 글자 크기를 'rem, em' 단위로 변환하여 사용한다.
* 16px == 1em or 1rem / em은 부모를 따라가며, rem은 자기자신을 기준으로 삼는 root이다. root em 이라고 해석하자.
* 'https://nekocalc.com/px-to-em-converter'

## color
* 'color:rgb(0,0,0);'
* 'color:rgba(0,0,0,0); a -> alpha 투명도
* 'color: #fffff; (FF 두개 당 R, G, B를 나타낸다.)
-> 0~9까지, A부터 F까지, 0123456789abcdef 총 16개의 단계로
R -> 16*16 -> F*F 로 표현되어 FF값을 가지고
G -> 16*16 -> F*F 로 표현되어 FF인 것이다.
B 도 이하동문

그러나 16비트 최댓값이 255이므로, 256이 최댓값이 될 수 없기 때문에 255가 최댓값이다.

FF중 첫번째 F는 채도 강도값을 의미하며, 두번째 F는 세부값을 의미한다
* 'color:#FFF; (코드가 중복될 경우 압축하여 쓴다.)
* "color:aqua;

## CSS 수열 선택자
### 수열선택자란?
* CSS에서 요소를 규칙적으로 선택하고자 할 때 사용하는 선택자
* :nth-child(n) 형태로 작성되며, 반복 패턴을 따라 자식이 2개 이상 있을 때 N번쨰 자식이란 개념으로 선택한다.
클래스와 아이디로 의미있는 이름을 짓기 적합한 대상이 아닌경우 이름을 짓지않고 css 선택이 가능해 다양한 경우에 유용하게 사용할 수 있다.
ex) li:nth-child(2){background-color: red;} 2개 이상의 목록 중 2번쨰 li을 선택하여 배경색을 적용하는 수열 선택자.

## HTML - FORM (블록태그)
사용자 입력/선택 요소 1개라도 등장 시 전체 영역을 'FORM' 묶어주기 **action, method, id** 필수
* 폼 안쪽 양식 종류가 그룹별로 2개 이상 구분 될 경우 'fieldset, legend' 작성한다.

## fieldset (블록태그)
* fieldset' 은 'div'처럼 그룹역할 이므로 id 또는 Class를 함께 작성해야한다.
* 'filedset' 생략하고 대신 'div, ul, ol, dl' 등 다른 그룹으로 대체하는 것도 가능하다.

## form - input (인라인 태그)
* "<input type="종류" name ="데이터명" id="데이터명"(중복X) class="공통 디자인명">"
* 'value' 속성은 필요한 경우만 작성, (ex) 쇼핑몰 수량 기본값 1

## input 버튼요소 button, input (인라인 태그)
<input type="button" vaule="기본">
<input type="submit" vaule="제출">
<input type="reset" vaule="초기화">

<button type="button">기본</button>
<button type="submit">제출</button>
<button type="reset">초기화</button>

<!-- button은 현재 창에서 다음 단계로 넘어가려고 할 때 쓰는 태그 -->
<!-- a는 현재 단계에 상관없이 다른 창이나 다른 사이트로 넘어갈 때 쓰는 태그-->
<!-- button 기능을 활성하기 위해 특정 조건 ex)login 이 필요할 경우 a태그를 쓰고 role속성으로 "button" 준다. -->