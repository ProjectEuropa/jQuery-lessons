## jQuery program 3 TODOリスト改良しよう

- TODOアプリを改良しよう
- ヒント


## TODOアプリを改良しよう
- TODOアプリのTODOリストに完了ボタンと削除ボタンをつけてみよう
- 完了ボタンをクリックすると訂正線がつくように、削除ボタンをクリックするとTODOが削除するようにしてみよう
- ドラッグアンドドロップでTODOリストを並び替えてみよう

## ヒント
```js
$("li").on("click", function(){
    var index = $("li").index(this); // ES2015以降は変数宣言はvarよりletやconstを使うことが多いです
    alert(index);
   // indexメソッドでセレクタの何番目にアクセスしたかが分かります。
});

var liText = $("li").eq(0).text();
alert(liText);
//eqメソッドでセレクタのN番目の要素を指定できます。(最初は１からではなく0から始まります)
```

## ヒント2
```js
//clickメソッドではなく
$(document).on("click" , セレクタ , function() { 
});
// 又は
$(セレクタ).on("click" , function() {) {
});
//を使ってみよう。

//clickメソッドはJavaScript読み込み完了後に動的に追加された要素には、イベントが発火しないためです。
```

## ヒント3
ドラッグアンドドロップについてはjQuery ui で調べてみよう
