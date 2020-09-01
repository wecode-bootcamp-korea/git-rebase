Hi!

# rebase에서 conflict가 발생하면 모든 커밋에서 conflict가 발생한다.
# 1. 충돌 해결
# 2. git add .
# 3. git rebase --continue (rebase를 이어서 진행한다는 의미다.)
git rebase --continue

# commit을 두 세번 정도 했으면 rebase와 squash를 돌리자.
# 왜냐면 commit이 계속 늘어났을 때 충돌해결을 그 갯수 만큼 엄청 해줘야 하기 때문이다.

# rebase 중 뭔가 잘못된 것 같을 때 멈추는 커맨드 (아예 처음으로 돌아간다.)
git rebase --abort

# history가 달라서 깃에서 오류를 알려주는 건데 이때 --force 옵션을 활용해서 push 하면 된다.
git push origin feature/~ --force