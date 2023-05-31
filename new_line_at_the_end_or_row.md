# New line at the end of row
The following codes are equivalent<br>
This:
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