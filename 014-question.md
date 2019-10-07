# 存在演算子

## 存在演算子の書き方
```
# money = 1000
result = if money? then "found" else "not found"
alert result // => not found
```

## 二項演算子
```
# money = 999
result = money ? 0
alert result // => 0
```

## 安全なアクセス演算子
```
user =
  name: "Sakura"

alert user.score?.English // => undefined
```

以上、便利なCoffeeScriptの `？` でした
