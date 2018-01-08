
## jQuery Ajax

## Ajaxとは
ブラウザ上でページを読み込み直すことなくサーバーと通信し、表示内容を動的に変える技術。

```js
// 書き方の例
$.ajax({
    url:"hoge.php", // 指定するURL
    type:"get", // httpメソッド
    data:{
        "hoge":$("#hoge").val() // 送信するパラメータ
        }
    })
    .done(function(data){
        console.log(data); // Ajaxが成功した時の処理 一般的にはサーバー側でJSONデータを送信して、JavaScript側でJSONを受け取る
    })
    .fail(function(){
        console.log("通信失敗"); // Ajaxが失敗した時の処理
    });

    // こういうシンプルな書き方もある
    $.ajax({
        url: "data/hoge.txt" // 指定するURL(textデータも読み込み可能)
    })
    .then(
        function (data) {
            console.log(data); // Ajaxが成功した時の処理
        },
        function () {
            alert("失敗") // Ajaxが失敗した時の処理
        });

    // オプション・その他のAjax通信方法などは様々な書き方があるので各々調べてください
```
