# 60_wrapBinarySearch

**What is meant by count = log2n ? Express its meaning in a .**
- count is the exponent to which 2 must be raised to yield n
- read "log base 2 of n" or "the logarithm of n to the base 2"


**What does its graph look like?**
- it looks like the curve of count = 2^n reflected about the line y = x.
- Domain: (0, infinity)
- Range: (-infinity, infinity)
- y-int: none
- x-int: 1
- asymptote: y-axis

Problem: To return the index of an occurrence of findMe in a list,
or -1 if findMe is not in the list.

Recursive abstraction: When I am asked to return the index of findMe in a list of size n,
the recursive abstraction can return the index of findMe in a list of size n/2.

Generalized recursive solution:
```
Is the lowLim greater than the highLim? // boolean deciding which sol to use
  If yes, return -2.                    // solution to base case
If no,
  if findMe is the middle page of the array, 
    return the page number.             // solution to other base case
  // recursive cases
  if findMe is before the middle page of the array,
    return 
      the result of applying these instructions to the first half of the array.    
  if findMe is after the middle page of the array,
    return
      the result of applying these instructions to the second half of the array.
    
 ```


