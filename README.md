## ハンバーガーメニューを自作する

```js
$(セレクタ).toggleClass("hoge");
// セレクタにclass="hoge"がなければclass="hoge"を追加、ある場合はclass="hoge"を削除する

$(セレクタ).slideToggle()
//セレクタ表示されている時は隠し、隠れている時は表示する
```

## 課題
drawer.htmlに対して
```html
<i class="fa fa-bars" aria-hidden="true" id="drawer"></i>
```
アイコンをクリックした際に、ナビゲーションメニューが開くようににしてください。ナビゲーションメニューが開いている時にアイコンをクリックするとナビゲーションメニューが閉じるようにしてください。またナビゲーションメニューが開いている時と閉じている時にアイコンを切り替えるようにしてください。

## 参考
jQueryリファレンス
http://www.jquerystudy.info/reference/effects/slideToggle.html　
http://www.jquerystudy.info/reference/attributes/toggleClass.html
