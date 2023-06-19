# Comparing floating point number
It is risky to compare floating point numbers with the == operator, because it
is possible that the values should be equal but they are not because of precision
errors
In practice, the numbers can be compared as follows (ε = 10−9 ):
```cpp
if (abs(a-b) < 1e-9) {
  // a and b are equal
}
```