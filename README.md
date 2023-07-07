# GPT_with_Line_in_English
* 先下載django，使用此架構方便進行程式撰寫
* django-admin startproject '專案名稱'
* python manage.py startapp 'APP名稱'
* 修改LINE的Channel Access Token跟Channel Secret
* 接著進行語系、時區的設定
* 最後是新增static路徑
* ALLOWED_HOSTS = ['*']
* 設定url.py檔案
* 進行資料庫遷移的初始化 ```python manage.py makemigrations```   and    ```python manage.py migrate```
* 後台建立一個管理者帳號```python manage.py createsuperuser```
* 創建LINE BOT APP 此次APP名稱為(help_app)
* 撰寫主程式到views.py檔案中
* 到line中連結webhook
    * 先啟動python(python3 manage.py runserver 0.0.0.0:8800)
    * 再啟動ngrok()
    * 把ngrok網址後面加上/callback後放入line webhook當中


* 啟動python server
    * 0.0.0.0包含這台所有的ip位置，包括127.0.0.1還有172.105.238.116(根據每台ip位置而改變)
```python3 manage.py runserver 0.0.0.0:8800```
* 在瀏覽器查詢中輸入```172.105.238.116:8800```




