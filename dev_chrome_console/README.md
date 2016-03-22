# Tips for using the console in Chrome

### Measure performance of a block
```
console.time('Addition');

let a = 5;
a++;

console.timeEnd('Addition');
```

### Format data you want to display as a table

```
console.table([{a: 1, b: 2, c: 3}, {a: "foo", b: false, c: undefined}])
```

### Display objects in a friendlier way

Instead of using ```console.log(obj)``` you can use ```console.dir(obj)```

Read more about the dev console [here](https://developer.chrome.com/devtools/docs/tips-and-tricks).
