# 2D Array
## Conventions
- `n` = number of rows
- `m` = number of columns
- `i=0 ... (n-1)` = index of each row
- `j=0 ... (m-1)` = index of each column
## Leading Diagonal
- `i=j`

## Trailing Diagonal
- `i+j=n=min(n,m)`

## Movement of ♜(rook)
- Horizontal: `i=const`
- Vertical: `j=const`

## Movement of ♝(bishop)
- Along leading diagonal: `i+j=const`
- Along trailing diagonal: `i-j=const`
- Problem: [621B - Codeforces](https://codeforces.com/problemset/problem/621/B)

## Color of a square in chessboard
- Parity of `(i+j)` represents the color of square
- `h1` (bottom right) is white
- Problem: [445A - Codeforces](https://codeforces.com/problemset/problem/445/A)