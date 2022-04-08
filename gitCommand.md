### Terminal 명령어

폴더 생성 `mkdir`

파일 생성  `touch <file name>`

파일 수정 `echo "컨텐츠"> file-name.txt`

히든 파일 표시 `ls -la`, Finder -> command + shift + .

파일 삭제 `rm <file name> rmdri <folder name>`

# Local Repo

### 버전체크

git --version

git status

### Homebrew 설치

```
https://brew.sh/index_ko
```

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

### git 설치

```null
brew install git
```

### git 초기화

git init

---

### 브랜치

`git branch -m Git-test-branch`

### Add & Commit

`git add <file name>`

`git add .`

`git commit -m "this is second time"`

---

### Merging Branch

메인 브랜치 체크아웃

`git merge Git-third-branch`

### HEAD

head = current branch

`cat .git/HEAD`

returns current branch

### Detached HEAD

`git log`

`copy head id`

`git checkout <head id>`

작업 후 새 브랜치 생성

`git switch -c <new branch name>`

### Switch Branch

`git switch <branch-name>`

`git switch -c <new-branch-name>`

### Undo stage

`git ls0files`

`rm a.file`

`git commit -m "message"`

### Unstage

`git restore --staged file.name`

`git restore --staged .`

`git restore .`

### Delete commit

`git ls-files`

`git status`

`git reset --soft HEAD~1`

`git reset HEAD~1`

`git reset head HEAD~1`

### Delete Branch

`git branch -D <branch-name>`

### .gitignore

> // 무시할 파일 이름
>
> a.txt
>
> *.txt
>
> *.log
>
> !main.js

> // 무시할 폴더 이름
>
> abc/*

# Remote Repo

### existing branch

`git remote add origin <github address>`

`git branch -M main`

`git push -u origin main`

### initial branch

`echo "basic" >> readme.md`

`git init`

`git add readme.md`

`git commit -m "first commit"`

`git branch -M main`

`git remote add origin <github address>`

`git push -u origin main`


### Pushing history and Branches

`git push origin main -u`

`git push`

`git branch -a`


### Remote Branch

`git branch -r`

### Track Remote Branch

`git fetch origin`

`git branch -r`

`git branch --track local-branch-name origin/target-remote-branch`

`git pull`


### Important commands

`git remote -v`

`git remote show origin`

`git branch -vv`

### Upstream

`git push -u origin branch/name`

### Delete remote branch

`git branch --delete --remote origin/branch-name`

`git remote-ls`

`git push origin --delete branch-name`

`git reset --hard HEAD~1`

`git push origin main`


### Fork Repo

fork

`git clone <git repository address>`

`git remote add upstream <git repository address>`
