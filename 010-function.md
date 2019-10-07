# function

## functionの宣言
jsの場合、
```
function hello() {
  alert("hello")
}
hello() // => hello

var bye = function() {
  alert("bye")
}
bye() // => bye
```

CoffeeScriptの場合、
```
hello = ->
  alert "hello"
hello() // => hello
```

## 引数の扱い
jsの場合、
```
function hello(name) {
  alert("hello " + name)
}
hello("Sakura") // => hello Sakura
```

CoffeeScriptの場合、
```
hello = (name) ->
  alert "hello #{name}"
hello "Sakura" // => hello Sakura
```

引数に初期値を指定したい場合はjsと同じく、
```
hello = (name = "Sakura") ->
  alert "hello #{name}"
hello() // => hello Sakura
```

## 返り値
CoffeeScriptは `return` を明記しなくても最後の値が返却値となる
```
hello = ->
  name = "Sakura"
  "hello #{name}"
alert hello() // => hello Sakura
```

## 即時関数
jsの場合、
```
(function() {
  alert "hello"
})();
```

CoffeeScriptの場合、
```
do -> alert "hello"
```
