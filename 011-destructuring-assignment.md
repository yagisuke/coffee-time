# 分割代入

## 分割代入の書き方
CoffeeScriptの場合、
```
[a, b, c] = [1, 2, 3]
alert a // => 1
alert b // => 2
alert c // => 3
```

関数の返却値を分割代入するとこんな感じ
```
results = (x) -> [x, x ** 2, x ** 3]
[a, b, c] = results 3
alert a // => 3
alert b // => 9
alert c // => 27
```

jsと同じくobjectの分割代入はこんな感じ
```
user =
  name: "taro"
  score: 5
  email: "taro@hanako.com"
{name, score} = user
alert "#{name}さんは、#{score}点です" // => taroさんは、5点です
```
