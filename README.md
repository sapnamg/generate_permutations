# Permutation Generator (recursive)
This repository contains a Python program that generates all permutations of numbers ```0``` through ```n-1``` (currently set to ```n=3```), using recursion. It was created as a class exercise to understand recursion and backtracking. Print statements are included throughout to show recursion depth and what happens at the end of each loop.

## How it works
1. Starts with an empty list representing a permutation.
2. Loops through numbers ```0``` to ```n-1```, appending a number if it does not yet exist in the current permutation.
3. After appending a number, the function recursively calls itself to run through the numbers again to continue building the permutation.
4. When the permutation reaches its target length, it is printed. The last number from the list is then removed (bactracking), so the function can try other numbers.
5. Each recursion prints the current depth and state for clarity.

## Snippet of output for n=3:
```
Entering Depth 0, current perm: []
Trying k=0
Appending and entering recursion for k=0
  Entering Depth 1, current perm: [0]
  Trying k=0
  k in perm
  Trying k=1
  Appending and entering recursion for k=1
    Entering Depth 2, current perm: [0, 1]
    Trying k=0
    k in perm
    Trying k=1
    k in perm
    Trying k=2
    Appending and entering recursion for k=2
      Entering Depth 3, current perm: [0, 1, 2]
New permutation: [0, 1, 2]
      Exiting Depth 3 due to found result
```
  (and so on)
