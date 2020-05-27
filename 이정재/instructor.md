git reset과 revert

#Reset
$ git reset<옵션> <돌아가고싶은 commit>

1. hard
$ git reset --hard <commit>
돌아가려는 이력 이후의 모든내용을 삭제

2. soft
$ git reset --soft <commit>
돌아가려는 이력으로는 돌아가지만 이후의 내용은 지워지지 않고, 인덱스는 그대로 있는 상태

3. mixed
$ git reset --mixed <commit>
돌아가려는 이력으로 돌아가며, 인덱스는 초기화

#Revert
$ git revert <commit>
이전의 이력은 그대로 있고, 새로운 commit이 생긴다.

협업시에는 reset보다는 revert가 더 유용하다.