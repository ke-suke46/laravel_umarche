## ダウンロード方法

git clone

git clone https://github.com/ke-suke46/laravel_umarche


git clone ブランチを指定してダウンロードする場合

git clone -b ブランチ名 https://github.com/ke-suke46/larvel_umarche

もしくはzipファイルでダウンロードしてください

## インストール方法

cd laravel_umarche

composer install

npm install

npm run dev

.env.example をコピーして .env ファイルを作成

.envファイルの中の下記をご利用の環境に合わせて変更してください。

DB_CONNECTION=mysql
DB_HOST=localhost
DB_PORT=8889
DB_DATABASE=laravel_umarche
DB_USERNAME=umarche
DB_PASSWORD=password123

XAMPP/MAMPまたは他の開発環境でDBを起動した後に

php artisan migrate:fresh --seed

と実行してください。(データベーステーブルとダミーデータが追加されればOK)

最後に
php artisan kiy:generate
と入力してキーを生成後、

php artisan serve
で簡易サーバーを立ち上げ、表示を確認してください。


## インストール後の実施事項

画像のダミーデータは
public/imagesフォルダ内に
sample1.jpg ~ sample6.jpg として
保存しています。

php artisan storage:link で
storageフォルダにリンク後、

storage/app/public/productsフォルダ内に
保存されると表示されます。
(productsフォルダがない場合は作成してください。)

ショップの画像も表示する場合は、
storage/app/public/shopsフォルダを作成し画像を保存してください。