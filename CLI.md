# CLI

## 新增.git資料夾

> 點Git Bash Here
> git init

## 查看可記錄的紀錄(顯示Unstage、Stage)
> git status

### 新增節點
將檔案從Unstage新增至Stage
> git add hello.txt world.txt
> git commit -m "Create file hello.txt and world.txt"

##### *從Stage返回至Unstage
>git restore --staged world.txt

### 查看commit的內容(log)
1. git log master
> 只顯示初行: git log master --oneline

### 回復至以前的節點
* git reset HEAD^
> ^表上一步, ^^表上兩步
* git reset 節點ID --soft
> soft: 資料回到Stage
> mixed: 資料回到Unstage(預設)
> hard: 刪掉資料

### 查看以前的節點(執行舊檔案, 保留現有新檔案)
* 跳至舊節點
> git checkout 節點ID
* 回到最新節點
> git checkout master


## 新增檔案
1. ls
2. touch hello.txt

### 新增檔案內容
1. echo "Hello world" > hello.txt