# React-Django App

基本コマンド

`docker-compose up --build`


### projectのはじまり

`django-admin.py startproject profiles_project .`

profiles_projectをcurrentdirで開始

- `profile_project` dirの生成
- `manage.py` が生成される


`profile_project`はプロジェクト全体の統括

プロジェクトが複数アプリケーションを持つこともよくあるのです


### 個別アプリケーションの作成

`python manage.py startapp profiles_api`

backend-api　projectの作成



### アプリケーションの登録

`project/setting.py` のinstalled appsへ

INSTALLED_APPS = [
```
    'rest_framework',
    'rest_framework.authtoken',
    'profiles_api',
```
の登録

### Check working!!

python manage.py runserver 0.0.0.0:8000



### Migration is 何？？

モデルに新たな属性を追加するたびにマイグレする必要があるよ

`python manage.py makemigrations profiles_api`

`python manage.py migrate`

### Memo

マウントするのあまり良くないのか？
