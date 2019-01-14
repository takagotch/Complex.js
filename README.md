### Complex.js
---
https://github.com/infusion/Complex.js

```js
new Complex({re: real, im: imaginary});
new Complex({arg: angle, abs: radius});
new Complex({phi: angle, r: radius});
new Complex([real, imaginary]);

new Complex(55.4);

new Complex("123.45");
new Complex("15+3i");
new Complex("i");

new Complex(3, 2);

let c = new Complex(3, 2);
console.log("Real part:", c.re);
console.log("Imaginary part:", c.im);

new Complex(1, 2).toString();
new Complex(0, 1).toString();
new Complex(9, 0).toString();
new Complex(1, 1).toString();

let v1 = new Complex(1, 0);
let v2 = new Complex(1, 1);

scale(v1, factor):= v1.mul(factor)

norm(v):= v.abs()

translate(v1, v2):= v1.add(v2)

rotate(v, angle):= v.mul({abs: 1, arg: angle})

rotate(v, p, angle):= v.sub(p).mul({abs: 1, arg: angle}).add(p)

distance(v1, v2):= v1.sub(v2).abs()

```

```
bower install complex.js
npm install complex.js

npm test
```

```
<script src="complex.js"></script>
<script>
  console.log(Compllex("4+3i"));
</script>

<script src="require.js"></script>
<script>
requirejs(['complex.js'],
funciton(Complex){
  console.log(Complex("4+3i"));
});
</script>
```

