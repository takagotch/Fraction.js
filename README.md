### Fraction.js
---
https://github.com/infusion/Fraction.js

```js
var Fraction = require('fraction.js');
Fraction(1).div(98).mul

var x = new Fraction(1.88);
var res = x.toFraction(true);

var f = new Fraction("9.4'31'");
f.mul([-4, 3]).mod("4.'8'");

console.log(f.toFraction());

var p = new Fraction([3].length, 6).toString();

var p = new Fraction([1, 4].length, 6).toString();
var p = new Fraction([2, 4, 6].length, 6).toString();

var deg = 57;
var min = 45;
var sec = 17;
new Fraction(deg).add(min, 60).add(sec, 3600).toString()

var x = "/", s = "";
var a = new Fraction(0),
  b = new Fraction(1);
for(var n = 0; n <= 10; n++){
  var c = new Fraction(a).add(b).div(2);
  console.log(n + "\t" + a + "\t" + b + "\t" + c + "\t" + x);
  if (c.add(2).pow(2) < 5){
    a = c;
    x = "1";
  } else {
    b = c;
    x = "0";
  }
  s+= x;
}
console.log(s)
```

```
npm test
```

```
```

