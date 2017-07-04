> 這是javascript 30 挑戰的第一天，From [wesbos](https://twitter.com/wesbos)的[repo](https://github.com/wesbos/JavaScript30)

# Chap 01 - JavaScript Drum Kit

* addEventListener 監聽事件
* audio HTML5
* css

```CSS
.keys {
  display: flex;
  flex: 1;
  min-height: 100vh;
  align-items: center;
  justify-content: center;
}

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

參考文獻：https://javascript30.com/
