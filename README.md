# Git 學習

## git 初始化

```sql=
$ git config --global user.name "Oli"
$ git config --global user.email "huang7179@gmail.com"

--查詢 git config 內容
$ git config -l

或是
$ more .gitconfig
```


## 常用指令

- git init  
建立新的本地端 Repository

- git status  
檢查本地端檔案異動狀態

- git add [檔案或資料夾]  
將指定的檔案（或資料夾）加入版本控制。用 git add . 可加入全部

- git commit -m "提交說明內容"  
提交（commit）目前的異動並透過 -m 參數設定摘要說明文字

- git log  
查看先前的 commit 記錄

- git push  
將本地端 Repository 的 commit 發佈到遠端

- git push -u origin [BRANCH_NAME]  
發佈至遠端指定的分支（Branch）





## Git Branch

git branch  
查看當前有什麼分支
    
git branch <branch_name>  
新增分支

git branch -D <branch_name>  
強制刪除

git checkout  
切換分支

git branch --delete dev  
刪除branch

git checkout -b <branch_name>  
在現有的commit底下，另外新增branch  
或是在新增新的branch後立刻切換到新分支  

git reflog (不常用)  
可以看到所有的分支內容，包括被刪除的分支

git branch -m <舊名字> <新名字>  
分支換名稱

git push -u origin master  
將本地推送到github

## git clone

```htmlembedded=
$ git clone <網址>
```

