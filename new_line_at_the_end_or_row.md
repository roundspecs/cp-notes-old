New line at the end of row
```c++
for(i = 1; i <= n; i++) {
  for(j = 1; j <= m; j++)
    cout << a[i][j] << " ";
  cout << "\n";
}
```
is equivalent to this:
```c++
for(i = 1; i <= n; i++)
  for(j = 1; j <= m; j++)
    cout << a[i][j] << " \n"[j == m];
```