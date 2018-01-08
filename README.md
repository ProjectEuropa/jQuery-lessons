## jQuery program  TODOリストを作ろう

- テキストボックスの値の取得
- テキストボックスから取得した値を
- htmlに書き込んでみよう
- appendメソッドについて
- Todoリストを作ってみよう


## テキストボックスの値の取得
```html
<body>
<input type="text" id="text-box" value="text">

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
</body>

<script>
var text = $("#text-box").val();
alert(text);
// $(セレクタ).val()でテキストボックスの値を取得することができます
</script>

```


## テキストボックスから取得した値をhtmlに書き込んでみよう

```html
<body>
<input type="text" id="text-box" value="text">
<div></div>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
</body>
<script>
var text = $("#text-box").val();
$("div").append("<div>" + text + "</div>");
</script>
```


## appendメソッドについて
```js
$(セレクタ). append(引数(htmlコード)); 
// appendは指定したセレクタの後に引数のhtmlコードが追加されます。
```

## 課題 TODOリストを作ってみよう

```html
実際のコード
<input type="text" id="todo">
    <button>write</button>
    <ul>
    </ul>

<!-- 上記のコードに対してボタンをクリックしたときに、ulタグにテキストボックスで入力した値がliタグで追加されるようなコードを記述してください。
 -->
```
