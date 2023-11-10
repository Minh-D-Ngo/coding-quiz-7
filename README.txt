Running Time of Algorithms
	- Time complexity: As mentioned in the question itself, if the the input
is an array of N elements, then the time complexity will be O(N^2).This is because 
the algorithm is using the Insertion Sort technique, and in the worst case (when 
the array is in reverse order), the inner loop may need to perform N/2 comparisons 
on average for each element, resulting in a quadratic time complexity.
	- Space complexity: The space complexity of the code is O(1) because it uses 
a constant amount of extra space regardless of the input size. The additional space 
is used for variables like shifts, key, and j, but these require constant space 
regardless of the size of the input array.

Ice Cream Parlor
	- Recursive Definition: Let count be a function that returns the number of 
combinations of two distinct flavors from the first i flavors whose costs sum up to
money. Then:
- Base Case: 	count(i, money) = 0 if i <= 0
		count(i, momey) = count(i-1, money) if i > 0
- Recursive case: count(i, money) = count(i-1, money) + count(i-1, money - arr[i-1)
if i > 0 and money >= array[i]
