--GitHub上傳--

檔案目錄右鍵 -> 
Open Git Bash here -> 
git init ->
git remote add origin (GitHub倉庫URL) -> 
git add . -> 
git commit -m "Initial commit(可以隨意修改""內的內容) -> 
git push -u origin 分支名稱(master或其他分支)

--修改URL--

首先確認URL是否正確:
git remote -v
設置正確的URL:
git remote set-url origin https://github.com/Chris920522/<你的倉庫名>.git
設置好後再次確認:
git remote -v

--查看有修改但還沒上傳的文件--

git status

--上傳所有修改後的檔案
git pull origin master --rebase
git add .
git commit -m "附加訊息或修改說明"
git push origin 分支名稱

--上傳修改後的單一檔案--

git add 檔案名稱(要加上副檔名) ->
git commit -m "附加訊息或修改說明" ->
git push origin 分支名稱

--恢復到未修改狀態(只能取消本地修改)--
git restore 檔案名稱(要加上副檔名)

--查看修改紀錄--
git log

--重置到指定修改紀錄--
git reset --hard 修改ID

--強制上傳到遠端倉庫(非必要避免使用，會覆蓋遠端倉庫的歷史)--
git push origin 分支名稱 --force

--下載遠端檔案--
git clone 倉庫連結.git
