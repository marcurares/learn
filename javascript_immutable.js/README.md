# Immutable.JS

#### Update object from a List:

```
list = list.update(
  list.findIndex(function(item) { 
    return item.get("name") === "third"; 
  }), function(item) {
    return item.set("count", 4);
  }
);
```

#### Deleting an item

Wrong:
```
this.state = this.state.delete('data').set('data', data);
```

Right:
```
this.state = this.state.delete('data').set('data', data);
```
Because set also does delete.
