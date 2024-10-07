# Technical Log - Number of Unequal Triplets in Array

## Overview

We have an array of positive integers in where we need to find and return the number of triplets that are distinct of each other and the selected numbers are in a increasing index order


## Context 

We have an 0-indexed array of positive integers nums provided by the problem. 
We need to find the number of triplets (i, j, k) that meet the following conditions :

- $0 <= i < j < k < nums.length$
- $nums[i] != nums[j]\quad nums[i] != nums[k]\quad nums[j] != nums[k]$

To finally return the number of triplets that meet the conditions. 

**Example 1**
Let's say that we have: 

Array = [1, 2, 3, 4]

Some of the triplets that compose the solution are :
- [1, 2, 3]
- [1, 2, 4]
- [1, 3, 4]

So the answer to the problem is 3

**Example 2**
Let's say that we have: 

Array = [1, 2, 2, 2]

In this example they are not the distinct numbers that follow the conditions said by the problem, so the answer to the problem is 0


## Solution 

After reviewing the problem statement, I began brainstorming potential solutions. However, before diving into any specific approach, I needed to assess the constraints to 
determine which ideas were worth pursuing. Upon checking the constraints, I noticed they were relatively small, which led me to consider a brute force approach as a 
straightforward and an easy solution.


So, how do we do it?

1. We need a loop for each index or element considered.
   * But because the conditions say that the element can not be the same, for the next loop we need to move one step ahead or index of the last index checked by the latest loop.
2. Then we need to only check wheter the three elements are distinct of each other,
   * if this is the case then we have found a valid triplet that can be part of the solution.



## Alternate solution 

An alternative approach to this problem could involve tracking the frequency of numbers and storing the index at which each number is found. While I haven’t fully developed 
this idea yet, I believe it’s a feasible solution.

