# 2023-hn-TaQuangLinh-GitPractice
--no-ff flag?
Về ý nghĩa, sự khác nhau của hotfix và release branch?
git clone: 
git log: check the commit history, by default: display the most recent commits.

--oneline: brief description
--graph: display merge history

git stash: Lưu các thay đổi mà chưa được commit. Lúc này có thể chuyển nhánh và làm việc khác.
git stash list: List of stashes.
git stash pop <stash@{n}>: Áp dụng cho stash gần nhất và xóa stash đó khỏi list.
git stash apply <stash@{n}>: Apply cho stash gần nhất. (Giữ nguyễn list)
git stash drop <stash@{n}>: delete stash in list.
git stash clear: delete all 



git reset <commit_id>: Quay lại commit chỉ định, tất cả mã nguồn thay đổi kể từ commit chỉ định đến commit hiện tại sẽ được để trong working directory.


git revert <commit_id>: Hoàn tác các thay đổi trong lịch sử commit.Đảo ngược các thay đổi từ commit chỉ định và tạo một revert commit mới.


git rebase <branch>: Nhận các thay đổi trên nhánh chính sang nhánh tính năng mà ko tạo một commit mới.


git cherry pick: Copy commit từ nhánh này sang cho nhánh khác.
checkout sang nhánh đích: git cherry-pick <commit_id>
