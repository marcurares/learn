# Reactive

>In computing, reactive programming is a programming paradigm oriented around data flows and the propagation of change. [Source](https://www.google.ro/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=0CCIQFjABahUKEwii7q6Up-_HAhWDxxQKHTYuD1g&url=https%3A%2F%2Fen.wikipedia.org%2Fwiki%2FReactive_programming&usg=AFQjCNFHMDRIfmm0ryMlnKpuMO3GDoOrdw&sig2=1Xx9UZHG9nF2OVfudIWF2g&bvm=bv.102537793,bs.2,d.bGg)

Thinking in Reactive

Not imperative

Asynchronous data streams

Streams can be: variables, user inputs, properties, caches, data structures.

#### Streams
* Sequence of ongoing events ordered in time
* Emit 3 things: value, error, "completed"

Listening to a stream is called *subscribing*.

The functions that listen: *observers*.

The streams that are being listen to: *observables*.

MetaStream = Stream of streams

#### Events
Events are captured **asynchronously**.

### Observer design pattern

>The observer pattern is a software design pattern in which an object, called the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods. It is mainly used to implement distributed event handling systems. [Source](https://en.wikipedia.org/wiki/Observer_pattern)

Observable = promise with multiple return values.
