# explain.how_to_jump_to_def.vscode
VSCode で PHP のコードジャンプ「定義元にジャンプ」をできるようにする方法を説明する。

![VSCode で PHP のコードジャンプ](./jump_to_def.vscode.gif)

## VSCode で PHP のコードジャンプをできるようにする
まず、以下の 2 つ拡張機能をインストールする。
- PHP IntelliSense
- PHP Intelephense

Ctr + Shift + P を押してコマンドパレットを開き「open settings json」と入力し、ユーザの settings.json を開く。

開いた settings.json には以下の内容を追記する

settings.json に追記:
```json
{
    "php.validate.executablePath": "＜php-win.exe へのパス＞",
    "php.executablePath": "＜php-win.exe へのパス＞",
    "php.suggest.basic": false
}
```

executablePath の例:
```
C:\\Users\\＜ユーザ名＞\\scoop\\apps\\php\\current\\php-win.exe
```
