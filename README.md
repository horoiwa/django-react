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

```
    'rest_framework',
    'rest_framework.authtoken',
    'profiles_api',
```
の登録
