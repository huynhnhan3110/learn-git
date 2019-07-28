# Coders Tokyo Git Course

## Git cheat sheet
* git init
* git status
* git add .
* git commit -m "content commit"
---
* git log // show time + content commit + key commit 
* git show // show content of new file after commit
* git diff // show content different code in file (old file)
---
* working directory // chua duoc git add .
* staging area // dang duoc git add chua duoc git commit
* git repository // da duoc commit
---
* git checkout // chua git add ma muon huy thay doi
* git reset // dang o trong staging area (da duoc add ) ma muon quay lai working directory (luc chua duoc add)
---
* git branch // xem tat ca cac nhanh
* git branch m1 // tao nhanh m1 
* git branch -d m1 // xoa nhanh m1

* git checkout -b thubay // tao 1 nhanh co ten la thu bay dong thoi chuyen minh sang nhanh do

* git checkout master // chuyen nhanh ve master ( se khong co nhung thu lien quan den nhanh thubay)
* git checkout m1 // chuyen lai nhanh m1
* git 

* nếu muốn gộp nhánh thì phải vào nhánh gốc rồi mới merge nhánh cần gộp
* git merge <nhánh cần gộp>
---
* git reset --soft <hash>// chuyển về staging area của commit trước
* git reset --mixed <hash> // chuyển về working directory của commit trước
* git reset --hard <hash> // xóa tất cả các commit từ hash trở về sau, giữ lại lại các commit trước hash. (Chú ý khi sử dụng)
---
* git revert <hash> // nó sẽ tạo cho mình một commit mới chứa cái mà hash chưa được commit. sau đó mình tiếp tục thêm vào cái mình muốn rồi commit lại nó sẽ theo quy tắc cầu thang, nó là bậc cao nhất. (hạn chế sử dụng nếu có nhiều edit trong một file) => nên làm bằng cách tạo 1 branch mới rồi chỉnh sửa trên branch đó rồi quay về branch master merge nó vào.
---
* .gitignore // dùng để bỏ folder khỏi staging area để không commit nó.
---
* git remote add origin <link co duoi .git> // kéo project mới tạo về để làm việc
* git push -u origin master // để push lần đầu tiên (yêu cầu username và pass để xác nhận)
* git push // để push những lần sau
---
* git config --global credential.helper store // save not encode in ~/git.credentials
* git config --global credential.helper "cache --timeout=18000" // sau 5 tiếng (1800s) sẽ yêu cầu nhập lại password
* git ssh
---
* git clone // clone 1 project nào đó chưa có trên máy mình để về làm việc
* git pull // ví dụ trên repo có thay đổi thì sau khi mình đã clone thì chỉ cần pull để nó update thay đổi đó cho project ở máy mình.
--- 
* git push origin <branch> // push branch lên trên github sau khi đã làm việc trên branch đó.
* git fetch origin <branch> // người reviewer gõ branch muốn kéo về để review code .

123
