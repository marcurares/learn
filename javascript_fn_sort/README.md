# Sorting an array in Javascript

You can easily sort an array in Javascript by usign the ```sort``` function.

```
[3, 1, 2].sort() //Will give you [1, 2, 3]
```

You can also specify a compare function

```
const compare = (a, b) => {
  if (a < b) {
    return -1;
  }

  if (a > b) {
    return 1;
  }

  if (a == b) {
    return 0;
  }
};

[3, 1, 2].sort(compare);
```

You can find more about the meaning of -1, 0, 1 here: [MDN - sort](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)
