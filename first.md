# GitHub Study

## GitHub 시작하기
* git 설치 후 gitbash프로그램(리눅스 명령어 사용가능)을 열어 $ git 명령어로 잘 설치되었는지 확인

명령어
>* $ git init : 현재 디렉토리에서 작업은 진행할 것임을 git에게 알려줌, 버전관리를 하고자 하는 폴더로 가서 git init을 입력하면 .git이라는 숨김파일이 생성
>* $ git add[파일명] : 해당 파일을 git이 관리할 대상으로 등록
> - 등록시 'LF will be replaced by CRLF in [파일명]' 과 같은 오류 발생시 -> $  git config --global core.autocrlf true (core.autocrlf 켜기)
>* $ git status : 프로젝트 폴더의 상태 확인

파일을 github에 올리기
>1. 저장소의 주소 복사
>2. 윈도우의 가져올 폴더에서 마우스 우클릭>git bash here로 git bash창 열기
>3. 깃을 처음 설치한 경우 처음에만 다음을 설정
>>  * $ git config --global user.name "여러분 깃허브 이름"
>> * $ git config --global user.email "여러분 이메일"
>4. $ git clone 복사한 저장소 주소 명령어를 통해 저장소 가져오기
