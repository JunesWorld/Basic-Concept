# Github 사용법

## Tip
- File 명은 동일하게 할 것
* Repository -> New -> Name
* 올리고 싶은 File 들어가기

## Install(Git Homepage)
- Homebrew : 설치되어 있어야한다.
- Xcode
  - Terminal : $ git --version
- Binary Installer
  - Download -> pkg 파일(다음으로 열기 -> 설치 프로그램 -> 열기)
- Windows
  - Git Homepage -> Download -> 자동 설치(모두 Next) -> 명령프롬프트 재부팅 후 git --version  

## VScode(원하는 Directory로 가서 작업)
- Terminal / git --version
- git init
- git config --global core.autocrlf input(MAC OS) / true(WINDOWS) // 개행 문자(Newline) 설정
- git config --global user.name '[GitHub 가입 ID]'
- git config --global user.email '[GitHub 가입 EMAIL]'
- git config --global --list // 등록 정보 확인(빠져나가기=q)
- git status // 버전 확인
- git add .a // 버전 관리
- git commit -m 'message'
- git remote add origin [repsitory 생성 주소]
- git push origin master

## Terminal
  1. git init
  2. git add -A
  3. git commit -m "first commit"
  4. git push

## Eclipse Upload
  1. Team -> Share project -> use or create check! -> create repository -> finish
  2. Github 주소 복사 -> Create Remote -> Configure Fetch -> Create -> Change
  3. User : Git 계정 / PW : Tocken 입력(Setting -> Develper Setting -> Personal Access Tockens -> Tockens(Classic) -> 저장 -> Expire -> 권한 모두 부여)
  4. Store in 체크! -> Finish -> Save & Fetch

## Delete
  1. Project Explorer -> Team -> Disconnect
  2. Git Repository -> Data and History 체크!

## Global User, Email Setting -> Terminal
  - git config --global user.name "[your_name]"
  - git config --global user.email "[your_email]"

## Setting Check!
- git config --list : user.name & email 잘 들어갔는지 확인!

## Untracked File
- git clean -fd
