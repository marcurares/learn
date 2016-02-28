# Handle both array / single element parameter in a function

[JSTIP](http://www.jstips.co/en/writing-a-single-method-for-arrays-and-a-single-element/)

Using this simple trick you will be able to pass both single objects and array to functions and still make them work the same.

```
function reverseWords(words) {
  let _words = [].concat(words);

  return _words.map((word) => word.split().reverse().join()a);
}
```

By using ```[].concat(words)``` our function will also work for a single element:

```
  reverseWords("hi") // ['ih']
  reverseWords(['abc', 'def']) // ['cba', 'fed']
```
