# Git Command

## Command

| 명령어 | 의미 |
|---|---|
| cd _`폴더 이름`_ | 디렉토리로 이동 |
| cd `.` | 현재 디렉토리 |
| cd `..` | 상위 디렉토리 |
| ls | 현재 경로 속 파일보기 |
| ls `-a` | 현재 경로 속 숨긴 파일까지 모두 보기 |
| pwd | 현재 경로를 확인하는 명령어 |
| touch `파일명.확장자명` | 파일을 만드는 명령어 |
| mkdir `이름` | 해당 이름의 폴더를 만듬 |
| rm `파일 이름` | 해당 파일 삭제 |
| rm -rf `폴더 이름` | 해당 폴더 삭제 |
| clear | 커맨드창 초기화 |

## Repository

(init, status, add, commit)

| 명령어 | 의미 |
|---|---|
| git add _`file1 file2`_ | file1 과 file2 를 추가함 |
| git commit -m _`"my message"`_ | my message와 함께 commit |
| git log | commit 정보를 확인해 볼 수 있음 |
| git commit --amend | git commit 수정 |

## Branch

(branch, switch, checkout)

| 명령어 | 의미 |
|---|---|
| git branch | branch 를 확인 |
| git branch _`branch name`_ | branch 를 만듬 |
| git switch _`'branch name'`_ | branch name 으로 전환함 |
| git switch -c _`branch name`_ | branch name 을 만들고 전환함 |
| git checkout _`branch name`_ | branch name 으로 전환 |
| git branch -d _`branch name`_ | branch 삭제 |
| bit branch -m _`branch name`_ | branch 이름 변경 |

## Marges

| 명령어 | 의미 |
|---|---|
| git marge _`branch name`_ | branch 병합 |