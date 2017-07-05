> 這是javascript 30 挑戰的第三篇，From [wesbos](https://twitter.com/wesbos)的[repo](https://github.com/wesbos/JavaScript30)

# 03 - CSS Variables

```CSS
:root {
  --base: #ffc600;
  --spacing: 10px;
  --blur: 10px;
}

img {
  padding: var(--spacing);
  background: var(--base);
  filter: blur(var(--blur));
}
```
* 在`:root`命名變數，我們也可以在任意的選擇器內命名變數。
* 自定義的CSS變數，開頭必須是兩個破折號 `--`
* 在要呼叫變數的選擇器裡面，使用`var()`呼叫該變數，跟function很像
  * `var()` 只能設定值，不能作為屬性的變數
  ```CSS
  .main {
    --side: margin-top;
    var(--side): 20px;
  }
  ```
  * `var()` 不能直接合併單位
  ```CSS
  .main {
    --gap: 20;
    margin-top: var(--gap)px;
  }
  ```
* JavaScript 讀寫 CSS 變數
  * 讀取： `getPropertyValue()`
  * 寫入： `setProperty()`

```Javascript
const suffix = this.dataset.sizing || '';
```
`dataset` 是該元素的所有 `data-` 的值

參考文獻：http://muki.tw/tech/native-css-variables/
