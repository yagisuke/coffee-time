# switch文
jsの場合、
```
val = "red";
switch (val) {
  case "red":
    alert("STOP");
    break;
  case "yellow":
    alert("CAUTION");
    break;
  case "blue":
  case "green":
    alert("GO");
    break;
  default:
    alert("wrong signal");
}
```

CoffeeScriptの場合、
```
val = "red"
switch val
  when "red"
    alert "STOP"
  when "yellow"
    alert "CAUTION"
  when "blue", "green"
    alert "GO"
  else
    alert "wrong signal"
```
