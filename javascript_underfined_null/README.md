# Javascript 'undefined' and 'null'

[JSTIP](http://www.jstips.co/en/differences-between-undefined-and-null/)

I will go a bit more in-depth

Firstly,

**Undefined**
```
A variable that has not been assigned a value is of type undefined. A method or statement also returns undefined if the variable that is being evaluated does not have an assigned value. A function returns undefined if a value was not returned.
```
Source: [MDN](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/undefined)

Worth reading: [History of undefined](http://www.2ality.com/2013/05/history-undefined.html)

**Null**
```
The value null is a JavaScript literal representing null or an "empty" value, i.e. no object value is present. It is one of JavaScript's primitive values.
```
Source: [MDN](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/null)

Worth reading: [typeof null](http://www.2ality.com/2013/10/typeof-null.html)

Main difference comes out of:

```
undefined (JSVAL_VOID) was the integer −2 ^ 30 (a number outside the integer range).

null (JSVAL_NULL) was the machine code NULL pointer. Or: an object type tag plus a reference that is zero.
```

Three more differences:
- Javascript does not set null, only undefined (not declared / declared but with no value)

- You can not have undefined in JSON, but you can have null

Worth having a short look over: [JSON standard](http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf). In the standard, it clearly states that
```
A JSON value can be an object, array, number, string, true, false, or null.
```
Source: [StackOverflow](http://stackoverflow.com/questions/13796751/json-undefined-value-type)

So this is why we can't use underfined.

- Both are falsy & [primitives](https://github.com/stefan-moraru/learn/tree/master/javascript_primitive)
