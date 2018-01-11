# jQuery lesson 1 - jQueryの基本

- jQueryとは
- 基本的な使い方
- jQueryの基本的な書き方
- よく使用するメソッド

 ## jQuery とは
- JavaScriptをより扱いやすくしたファイル集（通称：ライブラリ） 
- 素のJavaScriptより少ないコード量でHTML・CSSの要素の操作が可能
- アニメーション等WEBページにより動きを出す事に特化している


## 基本的な書き方
- jQueryのファイルを読み込む
（CDN・直接ダウンロードして配置・Node.jsを使用してビルド等）
- jQuery読み込み後にjQueryのコードをjsファイルまたはscriptタグ内に書き込む


## 実際に使ってみよう！(cdn使用)
```html
<body>
<p>Click me!</p>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
</body>

<script>
$("p").click(function(){
    $(this).hide();
});
</script>

```


## 外部ファイル読み読み

```html
<!-- HTMLファイル -->
<body>
    <p>Click me!</p>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
    <script src="sample.js"></script>
</body>
```
```js
// jsファイル
$("p").click(function(){
    $(this).hide();
});
```

## jQuery の基本的な書き方
```js
$(セレクタ).メソッド(引数); // セレクタとはhtmlの要素

//実際のコード
$("p").click(function(){
    // p タグに対してclickメソッドを適用する
    $(this).hide(); // クリックされた要素(this)を隠す
});

実際のコード
$("#sample").click(function(){
    // id=“sample”に対してclickメソッドを適用する
});

$(".sample").click(function(){
    // class=“sample”に対してclickメソッドを適用する
});
// タグやid, class等の要素を指定して、指定した要素に対して何らかしらのイベントを起こすのが基本的な使い方
```

## よく使用するメソッド（イベントハンドラ）
| メソッド（イベントハンドラ）       | 説明           |
| ------------- |:-------------:|
| click      | 選択した要素のclickイベント発生時に関数を実行する |
| hover      | 選択した要素のhoverイベント発生時に関数を実行する|
| change     | 選択した要素のchangeイベント発生時に関数を実行する|

## よく使用するメソッド（要素の操作）
| メソッド       | 説明           |
| ------------- |:-------------:|
| hide()     | 要素を非表示にする|
| show()      | 要素を表示する|
| add()     | 要素を追加する|

数えきれないほどのメソッドが存在するので、適宜ドキュメントを参照するか。Googleでやってみたいことを調べてみてください。


## 課題1

```html
<body>
    <p>show and hide me!</p>
    
    <button>show</button>
    <button>hide</button>    
</body>
<!-- 上記のコードに対して、showボタンを押したらp要素を表示し、hideボタンを押したらp要素を非表示にするコードを記述してください。
 -->
```

## 課題2
```html
<body>
    <div class="yellow">I am Yellow!</div>
    <div class="green">I am Green!</div> 
 </body>
<!-- 上記のコードに対して、class=“yellow”要素をマウスホバー時に黄色に、 class=“green”要素をマウスホバー時に緑色になるようにコードを記述してください。
 -->
```

## 課題3 
```html
<body>
    <div id="not-fade-out">Not fade out me!</div>
    <div id="fade-out">Fade out me!</div>
    
    <button>fade out</button>
</body>
<!-- 上記のコードに対して、id=“fade-out”要素をボタンダブルクリック時にフェードアウトするようにコードを記述してください
 -->
```

## 参考
- https://www.w3schools.com/jquery/default.asp
 （w3schools.com）
