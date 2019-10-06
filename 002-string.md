# String

## 文字連結
jsの場合
```
var score = 80;
alert("score: " + score);
```

CoffeeScriptの場合
```
score = 80
alert "score: #{score}"

# 計算することも
alert "score: #{score * 10}"
```

## 複数行
CoffeeScriptの場合
```
str = "
  This is a
  very long messge.
"
```

## heredoc
CoffeeScriptの場合
```
html = """
  <div id="mail">HELLO.</div>
"""
```