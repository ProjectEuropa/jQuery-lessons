## jQuery lesson 5 プラグインの作り方

```js
//作り方
$.fn.hoge = function () {
    alert("hoge")
    return this;
};

// 使い方
$(セレクタ).hoge();

// 具体例
$.fn.green = function() {
    this.css( "color", "green" );
    return this;
};
 
$("a").green(); // aタグが全て緑色になる
```

## 課題
plugin.htmlの「金額を入力してください」テキストボックス入力後に数値にカンマが自動的につくようなプラグインを作成してください。数値以外の文字列を入力した時は、テキストボックスの下にエラーメッセージを出すようにしてください。エラーメッセージ表示後に数値を入力した時はエラーメッセージが消えるようにしてください。

## 参考
http://learn.jquery.com/plugins/basic-plugin-creation/
