#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n)
As the size of n increases, the number of times the loop excutes increases linearly.

b) O(n**2)
The while loop nested inside the for loop will cause the time to increase exponentially.


c) O(n)
It's running a fixed number of times, where is bunnies (n) = 1, it would execute in O(1) time. The recursie call will execute n-1 total times, meaning the time to completion grows linearly with the increase of n as 1 + n-1.
Uses recursion, but each call only has one recursive call, like a single for loop.

## Exercise II

Use a Binary Search for an ordered list (floors).

Runtime complexity: O(log N)

Begin at the middle floor.

Start dropping eggs:
    Egg breaks, move to middle of bottom half.
        - Change top floor, or last floor, in comparison list to middle -1 floor.
    Egg doesn't break, move to middle of top half.
        - Change beginning to middle +1

Repeat process. Floor where eggs dropped begin to break will be at floor + 1 (one floor above), but not from current floor. 