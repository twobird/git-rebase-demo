# git-rebase-demo
git-rebase-demo


Git 版本控管實戰 - 課程實作進度回報

請先安裝好 Git 用戶端軟體，教學將會以 TortoiseGit 為主要工具，但其他工具的操作觀念都一樣，所以有興趣都可以試試：
1. 命令提示字元工具 ( Windows )

　Git for Windows
　http://git-scm.com/

2. 圖形化操作介面工具 ( Windows/Mac )

　TortoiseGit (Windows)
　https://code.google.com/p/tortoisegit

　GitHub Desktop ( 含 Git Shell 工具 )
　https://desktop.github.com/

分享文章

　30 天精通 Git 版本控管
　https://github.com/doggy8088/Learn-Git-in-30-days


設定 Git 必要的 user.name 與 user.email 設定

git config --global user.name <YourName>
git config --global user.email <YourEmail>

建立本地儲存庫

cd /d c:\
mkdir git-rebase-demo

cd git-rebase-demo
git init

echo TEST > D.txt
git add .
git commit -m "D"

echo TEST > E.txt
git add .
git commit -m "E"

git branch topic

echo TEST > F.txt
git add .
git commit -m "F"

echo TEST > G.txt
git add .
git commit -m "G"

echo TEST > H.txt
git add .
git commit -m "H"

git checkout topic

echo TEST > A.txt
git add .
git commit -m "A"

echo TEST > B.txt
git add .
git commit -m "B"

echo TEST > C.txt
git add .
git commit -m "C"


建立 GitHub 專案: git-rebase-demo

    https://github.com/new

複製 Git Repo 網址

    https://github.com/<github_id>/git-rebase-demo.git

加入 origin 遠端

    git remote add origin https://github.com/<github_id>/git-rebase-demo.git

    git remote -v

將本地儲存庫推上遠端儲存庫

    git push --all

建立所有遠端追蹤分支

    git fetch --all

練習 Merge 與 Rebase 操作
https://paper.dropbox.com/doc/-Merge-Rebase--G1JQ43VXWfhq6S05gSFSB


gitblit
http://gitblit.com/

GitLab
https://about.gitlab.com/

Fork my project
https://github.com/doggy8088/git-rebase-demo



練習主題 *
  00 安裝 Git 用戶端工具 & 註冊 GitHub 帳號並成功登入
 01 建立本日練習用 git 本地儲存庫 ( git-rebase-demo ) 並 push 到 GitHub 遠端儲存庫
 02 練習在遠端建立版本，並且 git fetch 回來，查看「遠端追蹤分支」的變化，在進行 git merge 合併，在最後用 Reset 復原本地與遠端版本
 03 練習 git cherry-pick 與 git revert 功能
 04 練習 Merge 與 Rebase 操作
 05 練習 git pull 的各種不同的合併方法
 06 練習最簡單的 GitHub Flow 版控流程
