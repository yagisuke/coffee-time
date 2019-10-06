# ループ

## for
jsの場合、
```
var sum = 0
for (var i = 0; i <= 10; i++) {
  sum += i;
}
alert(sum); // => 55
```

CoffeeScriptの場合、
```
sum = 0
for i in [0..10]
  sum += i
alert sum // => 55
```

CoffeeScriptforを後置して使う場合、
```
sum = 0
sum += i for i in [0..10]
alert sum // => 55
```

## 配列内包
CoffeeScriptは配列内包により、繰り返し行う処理の結果を配列にして返すことができる
```
sum = 0
total = (sum += i for i in [0..10])
alert total // => 0,1,3,6,10,15,21,28,36,45,55
```

CoffeeScriptに負けないように、今時のjsで書くとこんな感じ
(もっと格好いいのあったら教えてください)
```
let sum = 0
const total = [...Array(11).keys()].map(val => sum += val)
alert(total)
```

## while文
jsの場合、
```
var i = 0;
var sum = 0;
while (i < 11) {
  sum += i;
  i++;
}
alert(sum);
```

CoffeeScriptの場合、
```
i = 0
sum = 0
while i < 11
  sum += i
  i++
alert sum
```

CoffeeScriptのwhile文は最後に評価された値をまた配列で返却してくれる
```
i = 0
sum = while i < 11
  sum += i
  i++
alert sum // => 0,1,2,3,4,5,6,7,8,9,10
```