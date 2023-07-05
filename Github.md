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

## Clone
- 경로확인 : dir
- clone 원하는 Directory로 Go!
- git clone [Git Repository URL] 

## Code
- Cmd + Shift + P / Code 검색 명령 설치
  - 쉘 명령: PATH에 'code' 명령 설치
  - Shell Command: Install 'code' command in PATH
- VScode 재부팅
- Terminal : 폴더 Directory로 Go!
- `code . ` : 새로운 vscode에서 open
- `code . -r ` : 현재 vscode 창에서 open

## Version 관리
git-practice
- git init
- git add .
- git commit -m '1' // version1
- git log // version 확인
- 파일 수정 / git add . /  git commit -m '2' & '3'
- git reset --hard HEAD~1
  - 한 버전 돌아가겠다 = 2번 버전으로 돌아감
- git reset --hard ORIG_HEAD
  - 3번 버전으로 돌아감

## Branch 관리
- Terminal!
  - master 
- git branch
  - branch 목록 확인
  - 나가기 = q
  - git branch -a : 원격에 있는 branch 확인
- git branch [branch name] : branch 생성
- git checkout [branch name] : branch 변경
- 변경된 branch에서 작업
  - git add .
  - git commit -m 'message'
- git push origin [branch name]

[Git clone 후 Branch 가져오기]
- git branch -r : branch 확인
- git checkout -t origin/[확인한 branch명]

[Git clone 후 Branch 삭제하기]
- git checkout master
- git branch -d [삭제할 branch]

[Branch 생성 후 바로 그 branch로 가기]
- git checkout -b [branch name]

## Merge
- Github 저장소
- Pull Requests
  - new pull requests
  - base:master <--- compare:signin
  - create pull requests
  - create pull request
  - Merge pull Request
  - confirm merge

## 충돌
다른 환경에서 작업 후 push 했을 때 수정 부분 내용이 달라 충돌할 수 있다. <br />
- `git reset --hard HEAD~1`로 한 단계 복원
- git pull
  - 현재 변경 사항 vs 수신 변경 사항
  - 위에서 선택 가능!
- git status
- git add .
- git status
- git commit -m '수정 완료'
- git push origin master 

## NPX, Degit

새로운 Terminal Open

- 경로 확인
  ```bash
  ls
  ```
- 다운 받기 원하는 경로로 이동
  ```bash
  cd [원하는 경로]
  ```
- 설치
  ```bash
  npx degit [Github 이름]/[다운 받을 폴더 이름] [다운 시 원하는 폴더 이름]
  ```

## Git Push Error

Git: Can’t push refs to remote. Run ‘Pull’ first to integrate your changes.

```bash
git pull origin master
```

## VScode 10k 해결방법

현상 발생 이유 : .git 파일을 만들어 놓으면 발생

해결방법
```bash
cd /Users/june
ls -a
rm -r -f .git
```
