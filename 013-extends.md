# extends
CoffeeScriptの場合、
```
class User
  constructor: (@name) ->
    @message = "#{@name}さんこんにちわ／"
  hello: ->
    alert "hello #{@name}"

class AdminUser extends User
  hello: ->
    alert "admin says..."
    super()

tom = new AdminUser "Tom"
alert tom.message // => Tomさんこんにちわ／
tom.hello() // => admin says...
            // => hello Tom
```
