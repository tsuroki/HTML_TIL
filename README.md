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

##
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