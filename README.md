# GitHub Study

## GitHub 시작하기
### 시작하기 전에
* Git: 로컬 파일의 변경사항을 기록하고, 여러 사용자들과 작업하기 위한 버전 관리 시스템
* Github: 클라우드 방식으로 구현된 버전 관리 시스템, 즉 로컬 파일을 깃허브 클라우드에 업로드하여 사용하는 것

### Git설치하기
* 파일 다운 후 설치 진행 https://git-scm.com/download/
* git 설치 후 gitbash프로그램(리눅스 명령어 사용가능)을 열어 $ git 명령어로 잘 설치되었는지 확인

### 명령어
>* $ git init : 현재 디렉토리에서 작업은 진행할 것임을 git에게 알려줌, 버전관리를 하고자 하는 폴더로 가서 git init을 입력하면 .git이라는 숨김파일이 생성
>* $ git add[파일명] : 해당 파일을 git이 관리할 대상으로 등록
> - 등록시 'LF will be replaced by CRLF in [파일명]' 과 같은 오류 발생시 -> $  git config --global core.autocrlf true (core.autocrlf 켜기)
>* $ git status : 프로젝트 폴더의 상태 확인
>* $ git commit -m '[push메시지명]' : 첫번째 커밋을 만들음
>* $ git clone 복사한 저장소 주소 : 저장소 가져오기
>* $ git push -u origin master : 현재 브랜치를 원격저장소 origin의 master에 동기화함
>* $ git remote remove <원격저장소이름> : 원격저장소로 등록한 이름과 주소 삭제
>* $ git remote -v : 원격저장소 보기

### 파일을 github에 올리기
>1. 저장소의 주소 복사
>2. 윈도우의 가져올 폴더에서 마우스 우클릭>git bash here로 git bash창 열기
>3. 깃을 처음 설치한 경우 처음에만 다음을 설정
>> * $ git config --global user.name "여러분 깃허브 이름"
>> * $ git config --global user.email "여러분 이메일"
>4. $ git add [올릴 파일명]
>5. $ git commit -m '[push메시지명]'
>6. $ git remote add origin <원격저장주소> : 로컬 저장소에 원격저장소 등록, 주소가 길기 때문에 origin이라는 별명 붙여줌
>7. $ git push -u origin master :마스터브랜치 푸쉬
>>-u는 한번만 쓰면됨 이후엔 git push만 하면 자동으로 푸쉬시켜줌(로컬브랜치와 원격브랜치를 동기화) 
>8. 유저네임, 비밀번호 물어봄 > 입력 >푸시가 됨
> * 이후 파일 업로드시 4,5,7번만 반복
> ```
> * failed to push some refs to와 같은 오류가 발생하는 경우
> git push -f 옵션을 추가하여 강제로 push
> git pull 명령어로 원격 저장소 폴더의 파일을 내려받아 로컬 저장소의 폴더 파일과 같도록 한다 
> ```

### 업로드 한 파일 삭제
>* $ git rm [파일명] : 원격 저장소and로컬 저장소 파일 삭제
>* $ git rm --cached [파일명] : 원격 저장소에 있는 파일만 삭제
>* $ rm [파일명] : 로컬 에 있는 파일만 삭제
