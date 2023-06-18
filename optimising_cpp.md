# Optimizing CPP

- Use the follow commad to compile the code:
  ```sh
  g++ -std=c++11 -O2 -Wall test.cpp -o test
  ```
- Typing the following in your main function to make I/O more efficient
  ```cpp
  ios::sync_with_stdio(0);
  cin.tie(0);
  ```
- `"\n"` works faster than `endl`
