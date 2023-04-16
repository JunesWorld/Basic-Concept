# Github 사용법

- File 명은 동일하게 할 것
* Repository -> New -> Name
* 올리고 싶은 File 들어가기
## Terminal
  1. git init
  2. git add -A
  3. git commit -m "first commit"
  4. git push

## Upload
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
