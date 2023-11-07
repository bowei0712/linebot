# 安裝django套件
pip install django

# 建立專案
django-admin startproject appname(linebot1)

# 開啟目錄
- 檔案->打開資料夾(appname)

# 啟動Server(下完此指令，要再開一個終端機)
python manage.py runserver

# settings 設定網頁中文
LANGUAGE_CODE=''zh-Hant'
TIME_ZONE="Asia/Taipei"

# 新增功能
python manage.py startapp main

# 載入django.http套件(包裝成網頁要求)
from django.http import HttpResponse

'DIRS': [os.path.join(BASE_DIR, 'templates')]


python manage.py startapp test_html

#git指令
1.安裝git
2.專案目錄底下

# 初始化本地倉庫
- git init

#產生忽略檔案
-.gitignore

#檔案屬性
- U->UnTack
- A->Added
- M->Modifed (修改)

#加入控管
- git add <filename>
- git add . <加入所有未控管檔案/變動確認>

# 確認儲存
- git commit -m "message(做了什麼動作EX:初始化專案)"
- git commit -am "message" --am = add跟m一起使用

# 檢視狀態
- git status

# 檢視commit
- git log

# 綁定遠端倉庫
- git remote add origin https://github.com/bowei0712/linebot.git
remote(遙控) add(增加) origin(原點)
- git remote -v(帶出當下綁定的是哪個倉庫)

# 同步雲端倉庫
- git push -u origin master(第一次要這樣做)
- git push(第二次開始)

# 複製專案
- git clone https://github.com/bowei0712/linebot

# 同步專案
- python manage.py migrate