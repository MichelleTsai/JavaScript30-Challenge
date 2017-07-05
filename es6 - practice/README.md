# 從Chap 1 發想的模板練習

```Javascript
let name = 'Michelle', num1 = 4, num2 = 5;
let content = `My name is ${name} and my age is ${num1 + num2}`;
```
這裡可以在 `${}` 中間做`計算`也可以放`變數`，num 若沒定義則會 num is not defined(一樣加不成)

```Javascript
tag `My name is ${name} and my age is ${num1 + num2}`;

  0 : Array(3)
    0 : "My name is "
    1 : " and my age is "
    2 : ""
    length : 3
    raw : Array(3)
    __proto__ : Array(0)
  1 : "Michelle"
  2 : 9

  function tag(template){
    console.log(template);
  }
```
使用`標籤模版(tagged template)`，理解是把arguments放在tag所列出的array，index 與 index之間，等於是插入各個index之間

```Javascript

tag `My name is ${name} and my age is ${num1 + num2}`;

(2) ["Michelle", 9]
  0 : "Michelle"
  1 : 9
  length : 2

  function tag(template, ...values){
    console.log(values);
  }

```
利用其餘運算子，把arguments印出來，許多的參數轉換成一個陣列






參考文獻：https://pjchender.blogspot.tw/2017/01/javascript-es6-template-literalstagged.html
