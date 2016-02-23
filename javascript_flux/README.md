# Flux

* Dynamic data
* One way
* Dispatcher + event library

**Views dispatch actions**

## Dispatcher

* Event system
* Broadcasts events
* Registers callbacks
* Only 1 global dispatcher

## Store

Store responds to dispatched events

* Collection of data
* Singleton (see [Wikipedia](https://en.wikipedia.org/wiki/Singleton_pattern))
> In software engineering, the singleton pattern is a design pattern that restricts the instantiation of a class to one object. This is useful when exactly one object is needed to coordinate actions across the system.
* Stores emit "Change" events, to which views listen

```
var ListStore = {};

AppDispatcher.register(function() {
  switch(evName) {
    case 'foo':
      ListStore.push(bar);
      EventLibrary.emit('change');
      ..
  }
});
```

## Actions

* Abstraction on top of Dispatcher (easier to define, if there were no actions you would have to define cases in switch)

```
var ListActions = {
  add: () => {
    AppDispatcher.dispatch(..);
  }
};
```

## Flux scheme
![GitHub Logo](https://cask.scotch.io/2014/10/V70cSEC.png)

## Worth taking into consideration when thinking about using Flux

[Where Flux went wrong](http://technologyadvice.github.io/where-flux-went-wrong/)

TL:DR. Try to use state as little as possible, and rely more on props (this further abstracts the data source, hence an improvement). You can achieve this easily usign [Redux](http://redux.js.org/).
