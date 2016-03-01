# Javascript (ES6) template strings

Template strings are a cool feature added to ES6.

You can get rid of all the clutter that was around when strings where handled.

Normally:
```
  const x = 'abc' + a + ';' + b + ';' + c;
```

Or maybe even:
```
  const x = 'abc'.concat(a, ';', b, ';', c);
```

But with template strings, it's even easier:
```
  const x = `abc${a};${b};${c}`;
```

To use a variable inside a template string, just use it as: `${VAR}`.

Notice the use of ticks and not of apostrophes.

Read more about template strings here: [MDN](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/template_strings)
