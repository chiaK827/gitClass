# GUI_2

git > 版本控制
GitHub > 存放程式碼的平台

### 安裝git、fork
> https://git-scm.com/
> https://git-fork.com/

### octotree
> https://chrome.google.com/webstore/detail/octotree-github-code-tree/bkhaagjahfmjljalopjnoealnfndnagc


## 添加遠端
1. 複製Repository連結
2. 在Remotes右鍵Add New Remotes

### 將本地端檔案Push到GitHub上
1. Push
2. 選擇要上傳的分支
> Force push 不要鬧耶

### 將GitHub上的資料抓到本地端
1. Pull
2. 選擇從哪個遠端下載資料

### 將GitHub上的整體資料抓到本地端
1. 複製Repository連結
2. File > Clone
> 就是如果我本地端連資料夾都沒有的時候, 用Clone, 所以基本只有第一次會用到

### 遠端的資料與本地端的資料皆有變動時上傳資料
* 有小耳朵
1. Pull
2. Push
> 若遠端(GitHub)上的資料已經有更新, 名稱已經更改過, 所以會視為不同的名稱無法上傳, 所以需要將遠端的資料Pull到本地的資料, 並將兩邊的資料Merge(Fetch+Merge), 此時才可以Push

* 沒有小耳朵
1. Fetch
2. Pull > Rebase

### 合併分支(利用GitHub)
#### 提request
1. Pull requests
2. New pull requests
3. compare > 要合併至base的分支
4. Create pull request
5. 敘述(選填)
6. Create pull request

#### 通過request
1. Pull requests
2. 點要通過的request
3. Merge pull request
4. confirm merge
5. delete branch

#### 將merge的狀態傳回到本地端
1. Fetch
2. Remote下的master 拖至 Branches下的master
> Branches下的分支便可刪除了


### git flow
1. Repository > Git Flow > Initialize git flow
> 建立起git flow的環境(分支)
2. Repository > Git Flow > Start Feature
> 建立新功能
3. Finish 'feature/功能名稱'
> 將feature合併至develop
