# 60_wrapBinarySearch

## What is meant by y = log2x ?
2^y=x

## What does its graph look like?
The graph looks like an curve with an asymtote at x = 0 that increase rapidly at first but slows down.

## describe the recursive solution
0. Look for the index of a given value between that first and last indexes in the list using binary search.
1. If current page is less than the target page, look for the index between the current index + 1 and the upper index.
   If current page is greater than the target page, look for the index between the lower and the upper - 1 index.
2. Base cases:      If lower > upper, return -1
                    If current page is equal to the target page, return current page.
   Recursive cases: No combining element needed.
                    If current page is less than the target page, look for the index between the current index + 1 and the upper index.
                    If current page is greater than the target page, look for the index between the lower and the upper - 1 index.

