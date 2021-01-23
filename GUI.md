# GUI


✓master 表目前所在位置
### 回復至某節點
* 節點上右鍵Reset 'master' to here
> soft: 資料回到Stage
> mixed: 資料回到Unstage(預設)
> hard: 刪掉資料

* Revert Commit
> 該節點會失效, 但該點後面的節點仍有作用


### 各分支各自生長, 合併兩分支後會長成一個圈
1. merge > No-Fast Forward


### 合併兩分支後長成同一分支
1. rebase
2. merge > squash
3. Commit


### a在不合併分支的情況下, 取得b修改的檔案
1. 分支切至a
2. 在b修改檔案的節點上右鍵, Cherry-pick Commit
3. 完成


## 資料不上傳(敏感資料、測試檔)
1. 在資料夾建.gitignore
2. 在.gitignore中將不上傳的檔案名稱+副檔名填入