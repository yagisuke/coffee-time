# Object

# Objectの宣言
jsの場合、
```
var m = { name: "yagi", score: 40 };
```

CoffeeScriptの場合、
```
m = name: "yagi", score: 40
```

CoffeeScriptは改行して宣言することも
```
m =
  name: "yagi"
  score: 40

m =
  name: "yagi"
  score:
    Japanese: 10
    English: 60
    Chinese: 40
```