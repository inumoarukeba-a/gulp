# gulp

- babel + ES6
- browserSync
- sass
- pug
- cache
- watch
- notify
- plumber
- progeny
- rename
- replace
- frontNote
- image


## tasks

- `gulp` : 起動
- `gulp sass` : SCSSコンパイル
- `gulp js` : ES6 → ES5にトランスコンパイル
- `gulp pug` : pug → htmlにコンパイル
- `gulp note` : スタイルガイドを生成
- `gulp image` : 画像圧縮
- `gulp copy` : ルートと同階層に納品ファイル作成


## memo
- 20170213 : ES2016を使用出来るように修正（JSのファイル名は「~.es.js」）、frontnote（style集）導入
- 20170313 : 新規ファイルを追加しても、エラーで止まらないように修正（gulp.watch → gulp-watch に変更）
- 20170316 : 画像圧縮タスクを追加
- 20170330 : JPG圧縮にGuetzliを使用
- 20170406 : copy（納品ファイル作成）タスクを追加
- 20170411 : pugタスクを追加
- 20170421 : Png圧縮にpngquantを使用
- 20170515 : 画像圧縮のプラグインを変更

(1)` .babelrc`/`gulpfile.babel.js`を対象ディレクトリにコピー

(2) package.jsonを作成  
`npm init -y`

(3) プラグインをインストール
```
npm install -D gulp browser-sync babel-preset-es2015 babel-preset-es2016 gulp-sass gulp-pug gulp-cached gulp-notify gulp-plumber gulp-progeny gulp-babel gulp-rename gulp-replace gulp-frontnote gulp-watch gulp-image
```

(4) `gulpfile.babel.js`内のルートパスを変更
