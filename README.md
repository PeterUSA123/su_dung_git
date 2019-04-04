# Using Git

##  Tạo repo:

 ```git init```
 
## Config:

```git config --global user.name "Name" 
   git config --global user.email Email
   
   git config --local user.name "Name"
   git config --local user.email Email
   
   git config --list: Xem list config
```

 

## Add file, commit

``` git add <tên-tập-tin> 
    git add *
    git commit -m "Ghi chú Commit"
```

## Thêm nhánh, xóa nhánh, push nhánh lên remote, pull, merge

```git checkout -b feature_x: thêm nhánh
  
   git checkout <name branch>: chuyển nhánh
   
   git branch -D <name branch>: Xóa nhánh
   
   git push orgin <name branch>: Đẩy nhánh lên remote
   
   git pull: kéo về từ remote
  
   git merge A: đứng nhánh B muốn merge nhánh A
```

## git tag

```git tag <name tag> <commit>

   git log: show tag
```

## làm việc với thây đổi của file và commit

```git log: show all log commit

   git log --oneline, git log --pretty-oneline: show log với nhiều định dạng
   
   git reflog: show all log HEAD
   
   git reset <commit>: change position commit và xóa hết những commit phía trước
   
   git reset HEAD~N: thay đôi commit với N là commit muốn change, nếu muốn change cái hiện tại đang trỏ đến thì HEAD~
   
   git checkout HEAD@{N}:chuyển HEAD: 
   
   git checkout <commit> chuyển đến commit
   
   git reset --hard: xóa các thay đổi của tệp tin trước commit muốn trỏ tới
```
