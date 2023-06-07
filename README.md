# laravel-default
Laravel Project Initial Setup for 2023

## 概要
本リポジトリは2023年において、LaravelプロジェクトのデフォルトになるDocker-fileを用意したものである

# PHP

PHP | 8.1.11 

# TASK RUNNER

タスクランナーは別リポジトリに用意
Laravelとタスクランナーを結合したセットアップリポジトリは別に用意する

変更を加えるまではmainブランチで作業する
# STEP1
## dockerをbuildする
docker compose up -d --build

# STEP2
## composerからlaravelをインストールする

```
docker compose exec php bash
composer create-project --prefer-dist "laravel/laravel=" .
php artisan migrate
```

コンテナに入って
Laravelをインストール
DBをマイグレーション

# END
テスト
テスト
テスト
