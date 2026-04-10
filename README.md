# Product-of-Array-Except-Self
This C implementation solves the "Product of Array Except Self" problem by leveraging a Prefix and Suffix product strategy. The primary constraint is to achieve O(n) time complexity without using the division operator, which would otherwise fail if the array contained a zero.


Algorithm:
Prefix Pass: Create an output array where each index i stores the product of all elements from 0 to i-1.
Suffix Pass: Iterate backward from the end, maintaining a suffix variable. 
Multiply the value at each index i by the current suffix, then update the suffix by multiplying it with nums[i].
Return: The output array now contains the product of all elements except self for every position.
