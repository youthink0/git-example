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
    // 列出專案資料夾下的檔案和資料夾（-l 參數為列出詳細資料，-a 為列出隱藏資料夾  
    $ ls -la  
2.  
  git bash必須設定username及useremail，否則git無法提交資訊  
  指令為:  
    $ git config --global user.name "youthink0"  
    $ git config --global user.email [email protected]  
3.  
  日後要修改專案，雖然可以在github上直接修，但容易造成錯誤，建議把repo下載到local並修改完後，重新remote此資料夾並push(參照上述大致流程)  

tips:  
1.  
  創建好資料夾也初始化後直接把檔案丟進裡面，不要丟進.git  
  接著要 git add 檔案名字  
  用git status 確認有無變更  
2.  
  每次在本地修改完後，得輸入git commit -a -m "做了什麼事" 後，才能git push origin master  
3.  
  如果push出現error: failed to push some refs to ...  代表線上版本更新，需要 git pull --rebase後才能push  
4.  
  要移除檔案，請在local端輸入git rm -r 檔案名稱，接著push origin master即可  
5.  
  總流程複習 : git init -> git add 檔案名 -> git commit -a -m "message" -> git status確認狀態(非必要)  
  ->  git remote add origin github網址 -> git pull --rebase origin master -> git push origin master  
