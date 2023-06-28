# Operator function for sorting Struct
- The function takes on one parameter: `other`, the variable to be compared with
- The operator should return true if it is less that `other`

```cpp
struct P {
  int x, y;
  bool operator<(const P &other) {
    if (x != other.x) return x < other.x;
    else return y < other.y;
  }
};
```