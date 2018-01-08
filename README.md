## jQueryプラグインの作り方

```js
//作り方
$.fn.hoge = function () {
    alert("hoge")
    return this;
};

// 使い方
$(selector).hoge();

// 具体例
$.fn.green = function() {
    this.css( "color", "green" );
    return this;
};
 
$("a").green(); // aタグが全て緑色になる
```

## 参考
http://learn.jquery.com/plugins/basic-plugin-creation/
