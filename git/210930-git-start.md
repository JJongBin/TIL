# `git init`

git repo를 생성하고 순방향으로 cli를 이용해서 remote repo에 push하는 과정을 정리

- 프로젝트는 폴더 단위로 구분해야 하기 때문에 먼저 폴더를 생성해준다

1. 해당 폴더 내에서 `git init`을 입력해서 git을 사용할 수 있는 환경을 만든다
2. gitdl branch를 master에서 main으로 변경했기 때문에 변경해 준다 -> `git branch -M main` 
3. remote repo에 연결하기 위해 `git remote add [alias] [git-repo-src]`를 입력한다
4. 파일 작성 이후 `git add [file-name]`을 이용해서 stage에 파일을 올린다
5. local repo에 commit message와 함께 commit한다 -> `git commit` 
6. remote repo에 commit 내용을 밀어넣는다 -> `git push [alias] main`


# `clone`
repo를 생성하고, `git clone`을 이용해서 git과 연결
```
git clone [git-repo-src]
```

