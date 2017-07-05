> 這是javascript 30 挑戰的第一天，From [wesbos](https://twitter.com/wesbos)的[repo](https://github.com/wesbos/JavaScript30)

# Chap 01 - JavaScript Drum Kit

* addEventListener 監聽事件
* audio HTML5
* `transitionened`事件
* es6 forEach

`transitionened`事件，這個 transitionend 事件主要是對應到 CSS 中 transition 的動畫效果，當這個 transition 效果執行結束的時候會引發事件。

```Javascript
keys.forEach((key) => {key.addEventListener('transitionend', removeTransition)});
```

```CSS
.key {
  border: .4rem solid black;
  border-radius: .5rem;
  margin: 1rem;
  font-size: 1.5rem;
  padding: 1rem .5rem;
  transition: all .07s ease;
  width: 10rem;
  text-align: center;
  color: white;
  background: rgba(0,0,0,0.4);
  text-shadow: 0 0 .5rem black;
}

.playing {
  transform: scale(1.1);
  border-color: #ffc600;
  box-shadow: 0 0 1rem #ffc600;
}
```
+ `transform: scale(1.1);` 是把原本的東西放大1.1倍
+ `transition: all .07s ease;` 動畫表現在0.7秒內完成

參考文獻：https://javascript30.com/

練習模板字符串：
