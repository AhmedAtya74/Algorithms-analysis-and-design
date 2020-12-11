# Merge Sort

## Implementation for 2-way marge sort:
![image](https://user-images.githubusercontent.com/64374947/101917539-069ba780-3bd1-11eb-9438-39ff8d82c4be.png)
![image](https://user-images.githubusercontent.com/64374947/101917591-1915e100-3bd1-11eb-9ac1-737ec867a3dd.png)

## Algorithmic Paradigm:
> - Divide and Conquer algorithm.

## Recurrence relation:
> - T(n) = 2T(n/2) + θ(n)

## Time Complexity:
> - θ(nLogn) in all 3 cases (worst, average and best)

## Auxiliary Space:
> - O(n)

## Stable:
> - Yes

## Notes for 3-way marge sort:
> - we get the equation: T(n) = 3T(n/3) + O(n)
> - we get its complexity as O(n log 3n)
> - **Although time complexity looks less compared to 2 way merge sort, the time taken actually may become higher because number of comparisons in merge function go higher.**


## PROS of Merge sort:
> - Large size list
> - linked list 
> - External sorting

## Cons of Merge sort:
> - Extra Space (Not in-place)
> - Small problem
> - Recursive (Stack space)
