
## 네가 한 모든일을 알고 있다
```
$ git reflog
$ git reflog show <branch 이름>
$ git reset --hard <commit hash>
```

# 새로만든 파일까지 stash 시켜버리기
```
$ git stash -u
```

`git stash`는 수정된 파일만 stash를 시키고, 새로 만든 파일들은 unstage 상태로 남아있습니다. `-u` 옵션으로 모두 stash 시킬 수 있습니다.


# Common Sense of Git
- Always be committing
- Git stash for safety
