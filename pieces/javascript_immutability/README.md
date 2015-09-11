# Immutability

* Immutability
* Separation
* Composition
* Conservation

#### What is *immutability* ?

>The text-book definition of mutability is liable or subject to change or alteration. In programming, we use the word to mean objects whose state is allowed to change over time. An immutable value is the exact opposite – after it has been created, it can never change. [Source](http://www.sitepoint.com/immutability-javascript/)

So, after creation, an object cannot be changed.

In Javascript, strings are immutable, numbers too.

### Immutable.js
>Immutable data cannot be changed once created, leading to much simpler application development, no defensive copying, and enabling advanced memoization and change detection techniques with simple logic. Persistent data presents a mutative API which does not update the data in-place, but instead always yields new updated data. Immutable provides Persistent Immutable List, Stack, Map, OrderedMap, Set, OrderedSet and Record. They are highly efficient on modern JavaScript VMs by using structural sharing via hash maps tries and vector tries as popularized by Clojure and Scala, minimizing the need to copy or cache data. [Source](https://facebook.github.io/immutable-js/)

Setters don't change properties, they return a new object

A Set is an array with unique values.
A Map is an object with any kind of keys.

UpdateIn

A mutator is a setter.

### Memoization
>Memoization is a programming technique which attempts to increase a function’s performance by caching its previously computed results. [Source](http://www.sitepoint.com/implementing-memoization-in-javascript/)

A function caches the result for a given set of parameters, and, when the function is called, the first thing is done is to match the set of parameters against the cache. If the set is found in cache, the cached result is returned.
