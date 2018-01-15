## jQuery others 2 自作関数

- 自作関数
- デフォルト引数

JavaScriptでは関数を作ることで同じような処理処理をまとめることができる。
関数は変数と同じように宣言して作る。

```js
// 自作関数の例

/**
* 引数aとbを足して返却する
* @param Number 
* @param Number
* @return Number
*/
function sumApulsB(a, b) {
    retrun a + b;
}
```

ES2015以降では引数に初期値（デフォルト値）を設定することが可能になった。
デフォルト引数が設定されている引数が省略されて呼び出された際は、デフォルト引数が引数の値となる。

```js
// デフォルト引数の例

/**
* 引数aとbを足して返却する
* @param Number デフォルト値 1
* @param Number デフォルト値 1
* @return Number
*/
function sumApulsB(a = 1, b = 1) {
    retrun a + b;
}

sumApulsB();// return 2
sumApulsB(2, 3); // return 5
```
