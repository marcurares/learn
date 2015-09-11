# ES6
>ES6 is a significant update to the language, and the first update to the language since ES5 was standardized in 2009. Implementation of these features in major JavaScript engines is underway now. [link]
Always use const, use let only you know variable’s value is going to change. [Source](https://www.google.ro/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=0CCMQFjABahUKEwjv9-mnme_HAhUFuxQKHUrwB0M&url=https%3A%2F%2Fgithub.com%2Flukehoban%2Fes6features&usg=AFQjCNFjF5FvDoQhP4pDWHbe2vB2qzVr6A&sig2=bxNQw6xjADuIlk1KertX_g)

## Features
### Deconstructing
Left side of assignment

* Object example

```
var options = {
	repeat: true,
	save: false
};


var { repeat: localRepeat, save: localSave } = options;

var { keyName: variableName } = options;

//localRepeat = true
//localSave = false
```

* Array example

```
var array = [1,2,3,4,5];

var [ first, second ] = array;

//first = 1, second = 2
```

### Strings

**New features**: includes, startsWith, endsWith, repeat *( 'foo'.repeat(2) => 'foofoo')*

### Template strings

```
`string`
`string ${ javascriptExpression }`
```

### Default parameters

```
function (a = 'foo', b = 500, c = function() { }) { }
```

### Rest parameters

```
function (a, …restOfParams) {
  //restOfParams is an array with the rest of the parameters
}
```

### Deconstructing parameters

Useful for the function params being more readable / explicit

```
function setCookie(name, value, *{ secure, path, domain, expires }*) { }

setCookie('type', 'js', { secure: true,
    expires: 60000
});
```

### Object literals

```
{ foo: foo, baz: baz } is the same as { foo, baz }
```

### Methods

```
{
	methodName() {
		//..
	}
}
```

### Composed properties

```
{
  ['pro' + 'perty']: 'Something'
}
```
