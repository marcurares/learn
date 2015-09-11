# Javascript Good API Design

>[Information learned from this talk](https://www.youtube.com/watch?v=HYl7ReNB5TA)

#### Monolithic
Self-Contained

#### MicroServices
* Breaking up monolithic application
* Get increased decoupling
* Separation of concerns

### Good API
* Readable
* Consistent
* Crystal clear
* Prevent boolean traps
* Avoid confusing semantics
* Avoid double negatives *(const disabled = true should be const enabled = false)*
* Use verbal actions *(sendMessage is better than message)*


#### Static polymorphism
> We can generalize the concept to help us choosing the most optimal function and property names of a public interface. [Source](http://ariya.ofilabs.com/2014/03/api-names-and-static-polymorphism.html)

Example:
```
BAD
X1.value = 'Rare';
X2.value = 'Medium';
X3.value = 'Well done';
Y.option = 'Fries';
Z.caption = 'Order';

GOOD
X1.value = 'Rare';
X2.value = 'Medium';
X3.value = 'Well done';
Y.value = 'Fries';
Z.value = 'Order';
```

Basically, static polymorphism = constant names.

#### Explicit (im)mutability

```
point.translate(1, 1) //Should change p
point.translated(1, 1) //Should return a new object
```
