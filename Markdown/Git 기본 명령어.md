## Git 기본 명령어

```bash
$ git init
```



특정 폴더를 git저장소로 만들어 git으로 관리

- 특징

  폴더에 .git 폴더가 생성

  git bash에서는 (master)라는 표기를 확인할 수 있음

```bash
$ git add 
```



working directory에서 변경사항을 커밋하기 위해 staging area로 추가

- 특징

  파일의 상태가 staged로 변경됨

```bash
$ git commit
```



staging area에 있는 변경 목록을 .git directory에 업로드

- 특징
  - SHA-1 해시를 사용하여 40자 길이의 체크섬을 생성하고, 이를 고유한 커밋을 표기
  - 커밋 메시지는 변경 사항을 나타낼 수 있돌고 명확하게 작성해야 함

```bash
$ git status
```

- git 저장소에 있는 파일의 상태를 확인하기 위하여 활용

- 현재 저장소에 기록된 커밋을 조회

- 다양한 옵션을 통해 로그를 조회할 수 있음

  ```bash
  $ git log -1 # 최근 1개의 log
  $ git log -oneline # 한 줄로 log 표시
  $ git log -2 --oneline # 최근 2개의 log를 한줄로 표시
  ```



## 원격저장소 추가

```bash
$ git remote add <원격저장소이름> <주소>
$ git remote add origin https://github.com/<username>/<저장소이름>.git
```

- 원격저장소가 이미 설정된 경우 설정이 되지 않는다.(remote origin)

## 원격저장소 삭제

```bash
$ git remote rm <원격저장소이름>
```



## 원격저장소 push

```bash
$ git push <원격저장소이름> <브랜치이름>
$ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 215 bytes | 215.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Kim-Sunjin/test.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
```

- -u 옵션 : upstream 옵션
  - git push 라고 명령을 하더라도 설정된 원격저장소에 브랜치를 push
  - git push -u origin master

### 원격저장소 설정 명령어

```bash
$ git remote -v
```

- remote 확인 



```bash
$ git remote add <이름><url>
```

- remote 추가



```bash
$ git remote rm <이름>
```

- remote 삭제



```bash
$ git remote set-url <name><url>
```

- remoet url 변경



```bash
$ git remote renaem <이름><새이름>
```

- remote 이름 변경



### Branch

```bash
$ git branch <branch name>
$ git checkout master # master로 이동
$ git checkout branch name # branch로 이동
$ git checkout -b branch name
```

checkout 포인트를 만들어서 그 지점에서 branch 생성

master와 합칠 때 master branch에서 작성해야함

```bash
$ git merge branch name
```

