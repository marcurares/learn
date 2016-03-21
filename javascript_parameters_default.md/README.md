# Default parameters

This is a new feature included in ES6 (you can read more about es6 [here](https://nodejs.org/en/docs/es6/)). It allows you to specify default parameters for a function.

```
function echo(a) {
  console.log(a);
}
```

If you would invoke it like ```echo()```, you would get an error, because a is not defined.

Before es6, you would have to improve the function as:

```
function echo(a) {
  if (typeof a !== 'undefined') {
    console.log(a);
  }
}
```

With es6 default parameters, it can be easily written as:

```
function echo(a = '') {
  console.log(a);
}
```

The syntax is:
```
function fn(par1 = defaultValue1, par2 = defaultValu2) { ... }
```

Read more about default parameters [on MDN](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Functions/default_parameters).
