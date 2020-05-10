# git-example
learning how to use git repo


大致流程:
  在local創個專案(資料夾) -> 
  接著到github新增一個project -> 
  在git bash的terminal上cd到該專案 -> 
  輸入 git remote add origin "該project的url" //連線遠端github專案  -> 
  輸入 git push -u origin master //將本地專案更新到github專案上去 ->
  Done

Note:
1.
  local創project流程為:
    // 建立一個 name 資料夾
    $ mkdir name
    // 移動到 name 這個資料夾
    $ cd name
    // 將專案資料夾建立成 git repository
    $ git init
    // 列出專案資料夾下的檔案和資料夾（-l 參數為列出詳細資料，-a 為列出隱藏資料夾）
    $ ls -la
2.
  git bash必須設定username及useremail，否則git無法提交資訊
  指令為:
    $ git config --global user.name "youthink0"
    $ git config --global user.email [email protected]