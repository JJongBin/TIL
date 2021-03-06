# `git init`

git 설정을 먼저 해준다
- git config --global user.name "name"
- git config --global user.email "email"
- git config --global core.pager "cat"
- git config --global core.editor "vim"


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

# 권장하지 않는 사항
1. `git add .`: 잘못할 경우 필요하지 않은 다른 파일들이 추가된다  
2. `git commit -m ""`: 여러줄로 작성하던중 윗줄을 잘못 작성했을 경우 되돌릴 수 없다 -> 처음부터 다시 작성해야 한다
