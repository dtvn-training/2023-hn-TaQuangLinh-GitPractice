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


Tag:
	- Là một con trỏ tới một commit
	- Thường được sử dụng để đánh dấu các điểm release
	- Lighweight tags: Trỏ đến một commit cụ thể
	- Annotated tags: Đánh dấu các commit release, lưu nhiều loại dữ liệu hơn như: tagger name, email, date, tag message
git tag <tag_name> <
git tag -a <tag_name> -m "tag_message"
git show <tag_name>: display info of tag
git push <remote> <tag_name>: push a tag


Squash: Kết hợp nhiều commit thành một. Được thực hiện khi merge nhánh.
Có 2 cách để squash commit: 
- git rebase -i
- git merge --squash
