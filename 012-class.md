# class
CoffeeScriptの場合、
```
class User
  constructor: (@name) ->
    @message = "#{@name}さんこんにちわ／"
  hello: -> alert "hello #{@name}"

tom = new User "Tom"
alert tom.message // => Tomさんこんにちわ／
tom.hello() // => hello Tom
```
