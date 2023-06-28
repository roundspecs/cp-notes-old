# Map

### Declaration
```cpp
map<type,type> m;
map<type,type> m = {{key1,val1},{key1,val1}};
```

### Insert `O(log(n))`
```cpp
m.insert({key,val});
m[key]=val;
```

### Access
```cpp
m.at(key);
m[key];
```
### Exist/Count `O(log(n))`
```cpp
m.count(key) // 1 if exits, 0 otherwise
```

### Size `O(1)`
```cpp
m.size();
```

### Iterate
```cpp
for(auto [key,val]:m) {
  // ...
}
```

### Remove
```cpp
m.erase(key);
```

### Clear
```cpp
m.clear();
```