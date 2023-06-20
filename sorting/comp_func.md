# Comparator Function
Making comparator functions for sorting can sometimes seem confusing. So, to avoid confusion, think of `comp(a,b)` as `is_a_before_b(a,b)`

## Example: Sort string in terms of length first, then lexicographically
```cpp
bool comp(string a, string b) {
  if(a.size()==b.size()) return a<b;
  else return a.size() < b.size();
}

sort(a,a+n,comp);
```
