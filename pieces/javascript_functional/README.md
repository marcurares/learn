# Functional revolution

#### Innovation around functional programming.

## Functional programming
* Style of programming
* Discourages use of imperative programming
* Functions are the heart of it
* Data mutations should be avoided

### In Javascript

Functions are **first class citizens** (they can pe passed around as parameters, returned etc)

Composability = break code in small specialized units, that are reusable

Pure function = functions that do not mutate data and have no side-effects

High order function = function that takes a function as a param and returns a function


#### Functional programming at application level

Time
Asynchronicity
Promises = object wrapping a future result

#### Functional reactive programming

Streams

UI
* Predictable
* Composable

Components divide UI into small bits

#### Functional programming for front-end applications

* An app has a state
* State rendered in a tree of components, using the virtual dom
* The UI will generate events from user interactions, which will update the application state
* After the state update, the UI will be updated
