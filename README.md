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

requirejs(['fraction.js'],
function(Fraction){
  console.log(Fraction("123/456"));
});

console.log(Fraction("123/456"));

Fraction.REDUCE = <true|false>

var f = Fraction(3, 6);
console.log(f);
Fraction.REDUCE = false;
var g = Fraction(3, 6);
console.log(g);
Fraction.REDUCE = true;
var h = Fraction(g);
console.log(h);

var f = new Fraction('88/33');
var c = f.toContinued();

var f = new Fraction('-1/2');
console.log(f,n);
console.log(f.d);
console.log(f.s);

function formatDecimal(str){
  var comma, pre, offset, pad, times, repeat;
  if (-1 === (comma = str.indexOf(".")))
    return str;
  pre = str.substr(0, comma + 1);
  str = str.substr(comma + 1);
  for (var i = 0; i < str.length; i++){
    offset = str.substr(0, i);
  for (var j = 0; j < 5; j++){
    pad = str.substr(i, j + 1);
    times = Math.ceil((str.length - offset.length) / pad.length);
    repeat = new Array(times + 1).join(pad);
    if (0 === (offset + repeat).indexOf(str)){
      return pre + offset + "(" + pad + ")";
    }
  }
  }
  return null;
}
var f, x = formatDecimal("13.000000000");
if(x !== null){
  f = new Fraction(x);
}

new Fraction(3, 2);

var f = new Fraction("123.32");
console.log("Bam: " + f.div("33.6(567)"));

new Fraction("123.45");
new Fraction("123/45");
new Fraction("123:45");
new Fraction("4 123/45");

new Fraction(numerator, denominator);
new Fraction([numerator, denominator]);
new Fraction({n: numerator, d: denominator});

new Fraction(123);

var a = -1;
var b = 10.99;
console.log(new Fraction(a)
  .mod(b));
console.log(new Fraction(a)
  .mod(b).add(b).mod(b));

```

```
npm test

bower install fraction.js
npm istall fraction.js
```

```
```

