## 概要

コードフォーマッタツール

ESLintにも似たような機能があるがprettierのほうが得意としている

## インストール

```
npm install -D prettier
```

## 設定ファイル（.prettierrc）作成

```
{
    "tabWidth": 4,
    "singleQuote": true,
    "semi": true
}
```

## 実行

```
node_modules/.bin/prettier --write app.js
```

## package.json設定

```
  "scripts": {
    "format": "prettier --write app.js"
  }

  npm run format

  or

  yarn format
```

## vscode拡張機能

下記を実施すれば保存のたびに自動で整形してくれるようになる

1. プラグイン「Prettier」を導入
2. ctrl shift fからprettierをフォーマッタとして設定
   設定のデフォルトformatterからでも設定できる
3. 設定のonsaveを有効化
動かんかったら色々いじる

    settings.json

```
{
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "esbenp.prettier-vscode"
}
```
