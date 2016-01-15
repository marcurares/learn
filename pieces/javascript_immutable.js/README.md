# Immutable.JS

Update object from a List:

```
list = list.update(
  list.findIndex(function(item) { 
    return item.get("name") === "third"; 
  }), function(item) {
    return item.set("count", 4);
  }
);
```
