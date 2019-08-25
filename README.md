# Largest-Sum-Contiguous-Subarray
Simple idea of the Kadane’s algorithm is to look for all positive contiguous segments of the array.
Keep track of maximum sum contiguous segment among all positive segments.
Each time we get a positive sum compare it with max_current and update max_global if it is greater than max_global.
Lets take the example:
[-2,3,2,-1]
[-2,3,2,-2,5,4]
for i=0 a[0]=-2
max_current=max(a[0],max_current+a[i)
max_current=max(-2,-2+3)=1
set max_current=1 
max_current=max(-2,2+3)=5 
set max_current=5 and compare with max_global if greater than max_current then assign into max_global.
This is known as kadane's algorithm.
