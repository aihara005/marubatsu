## ゲームのアルゴリズム勉強用リポジトリ

* 最短でそのゲームのアルゴリズムを実現する

## 動作確認環境
* Laravel5.5
* PHP 7.2
* Apache 2.4.*
* MySQL 5.6

## 使い方
git clone https://github.com/aihara005/gameplac.git
composer install
yarn install
php artisan serve
localhost:3000へアクセス

### / ： ○☓ゲーム(3 ✕ 3)
最低限

### /othello : オセロゲーム( 8 ✕ 8)

#### 機能：
* Reset(デフォルトで2つずつ駒を置いた状態にする)
* Input（空いてるマスにコマを置き、他のコマを反転させる）
* Pass(自分の番をSkipする)

#### 設計：
* Controller: エントリーポイント
* Service：　ビジネスロジック(置かれたマスに対してその列のコマを反転させるかどうかなど)
* Repository: コマなどデータに関わる操作全て
