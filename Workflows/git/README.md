# 오늘의 깃팁

# Undoing

## 최근 커밋 메시지 바꾸기
```
$ git commit --amend
```

사실 커밋은 immutable하기 때문에 커밋 오브젝트가 바뀌는 것은 아님. `git commit --amend`로 커밋메시지를 수정하면 새로운 커밋 오브젝트가 생기고(hash값이 바뀌는 것을 확인할 수 있음), 업데이트 되는 것임. `git reflog`하면 HEAD(Local)에서 작업한 기록이 모두 남아있음.

## 수정한 파일 최근 커밋 메시지에 포함시키기
```
$ git add <수정된 파일>
$ git commit --amend --no-edit
```

`--no-edit` 옵션을 넣으면 커밋 메시지 수정없이 staged files를 커밋에 포함시킴.

## 방금한 커밋 취소하기 
```
$ git reset --soft HEAD^
```

`HEAD`는 항상 현재 branch를 의미하고, `HEAD^`는 하나의 커밋 전(parent commit)을 의미함. `--soft`는 file을 stage 상태로 보존하겠다는 의미함.

```
$ git config --global alias.uncommit 'reset --soft HEAD^'
```

## Stage된 파일 Unstage로 바꾸기
```
$ git status --short
M README.md
A app.py

$ git reset app.py

```
