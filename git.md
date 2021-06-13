### git testing 

#### git sync 
```
git pull
git staus
git add .
git commit -m "commit msg"
git push origin master

```



#### git first
```
mkdir demo
cd demo
git init
touch README.md
git add README.md
git commit -m "first commit"


````

```
git config --global user.name "用戶姓名" git config --global user.email "用戶Email" git config --list //確認"name"、"Email"有無打錯 git init //建立紀錄版本的數據庫(建立".git"檔案) git status //觀看是否有檔案沒有加到索引 git add index.html //發現"index.html"沒加到索引，於是將他加到索引，也就是加到觀察對象 git commit -m "first" //提交版本，並命名為 "first" git status //重新確認檔案有沒有加到索引 git log //看版本紀錄，這時應該只有 "first" //再來，下面的 git remote 選一個就好 //複製SSH網址，但要設定過SSH金鑰才能用 git remote add origin git@github.com:whalefine/xxxxxxxx.git //或是複製HTTPS網址 git remote add origin https://github.com/whalefine/xxxxxxxx.git git push -u origin master //把檔案push到github上 //若push遇到錯誤了 //可以輸入 git pull --rebase origin master //這樣就拿到雲端上的檔案了，再去push git push -u origin master //再不行就輸入下面這行 git push -f origin master

```


#### question
at win10 push by htts 
- git bash - push was failed, no any msg
- Sourcetree - also failed


#### Source 
> https://ithelp.ithome.com.tw/articles/10254114

> https://git-scm.com/book/zh-tw/v2/Git-%E5%9F%BA%E7%A4%8E-%E8%88%87%E9%81%A0%E7%AB%AF%E5%8D%94%E5%90%8C%E5%B7%A5%E4%BD%9C  基礎- 遠端協作
