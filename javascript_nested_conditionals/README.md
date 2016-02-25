# Nested conditionals improvement

[JSTIP](http://www.jstips.co/en/improve-nested-conditionals/)

Most of the info here is taken from that JSTIP.

Conditionals can get pretty big and tangled, so we have to get rid of the bloat. If you have a conditional like:

```
if (x) {
  if (x === 'a') {
    return function_a();
  } else if (x === 'b') {
    return function_b();
  } else if (x === 'c') {
    return function_c();
  }
}
```

You can get rid of it by using objects:

```
const cond = {
  'a': function_a,
  'b': function_b,
  'c': function_c
};

if (x in cond) {
  return cond[x]();
}
```

More about the ```in``` operator here: [MDN - in operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/in).
