## Exercise I

```
a) O(n^3) - the amount of computations is equal to (n * n * n). The count
starts at 0 and stops at 1 less than (n * n * n) because (a < (n * n * n)).

b) O(n^4) - there are 4 for loops that loops through n so that means
(n * n * n * n)

c) O(n) - the function runs recursively for n amount of times. It starts off at n and decrements by 1 each time until we reach 0.
```

## Exercise II

```
floors = [i+1 for i in range(n)]

- (mid = floors / 2) - Start with the middle of min and max and split the bottom and top floors into 2 seperate arrays.
- lower_floors = floors[:mid+1] - lower floors includes mid
- top_floors = floors[mid+1:] - top floors is everything above mid
- if the egg breaks do the same test on the lower floor.
- if the egg doesn't break do the test again on the top floor
- this problem can be solved using a binary search which has a runtime complexity of O(log n)
```
