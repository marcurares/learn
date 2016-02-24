# The 'splice' function

The splice function add / removes elements in an array at a given position.

```
let arr = [1, 2, 3, 4, 5];

arr.splice(pos, count, [new])

arr = [1, 2, 3, 4, 5];
arr.splice(0, 1); //[2, 3, 4, 5]

arr = [1, 2, 3, 4, 5];
arr.splice(0); //[]

//Basically removes item from pos to the end of the array

arr = [1, 2, 3, 4, 5];
arr.splice(0, 1, 100); //[100, 2, 3, 4, 5]
```

If count is omitted, it will be arr.length - start.
