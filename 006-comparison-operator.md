# 比較演算子や真偽値

## 比較演算子
CoffeeScriptでは以下のように書く。
ただしjsと異なり厳密等価/厳密不等価となる。
- 等価: `==` か `is`
- 不等価: `!==` か `isnt`

```
a = 100
b = 101
if a == b then alert "hello"
if a isnt b then alert "bye"
```

## 比較演算子の連結
jsの場合、
```
a = 50
if (0 < a && a < 100) {
  alert("GOOD");
}
```

CoffeeScriptの場合はこのように書ける
```
a = 50
if 0 < a < 100
  alert "GOOD"
```

## 真偽値
CoffeeScriptの真偽値は何個か書き方がある
- true: yes, on
- false: no, off

```
a = true
b = yes
c = on
if a == b == c then alert "GOOD" // => GOOD

d = false
e = no
c = off
if d == e == c then alert "GOOD" // => GOOD
```

## 論理演算子
CoffeeScriptの論理演算子は何個か書き方がある
- &&: and
- ||: or
- !: not

```
if true && true and true then alert "GOOD" // => GOOD
if true || true or true then alert "GOOD" // => GOOD
if !false && not false then alert "GOOD" // => GOOD
```

## その他
in: 配列の中に特定の値があるかどうか
```
TARGET_VALUE = 5
alert "GOOD" if TARGET_VALUE in [1..10] // => GOOD
```

of: オブジェクトの中に特定のkeyがあるかどうか
```
obj = score: 100
if "score" of obj then alert "GOOD"
```
