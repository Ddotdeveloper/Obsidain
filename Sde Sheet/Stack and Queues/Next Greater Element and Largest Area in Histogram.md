





### Largest Area of Histogram -:

##### Question
Find the largest rectangular area possible in a given [histogram](https://www.geeksforgeeks.org/histogram/) where the largest rectangle can be made of a number of contiguous bars whose heights are given in an array. For simplicity, assume that all bars have the same width and the width is 1 unit. 

****Example:**** 

> 	****Input:**** hist = {60, 20, 50, 40, 10, 50, 60}
> 	
> 	![Largest-Rectangular-Area-in-a-Histogram](https://media.geeksforgeeks.org/wp-content/uploads/20240924161857/Largest-Rectangular-Area-in-a-Histogram.webp)
> 	
> 	****Output:**** 100  
> 	****Explanation**** : We get the maximum are by picking bars highlighted above in green (50, and 60). The area is computed (smallest height) * (no. of the picked bars) = 50* 2 = 100
> 	
> 	****Input:**** hist = {3, 5, 1, 7, 5, 9}  
> 	****Output:**** 15  
> 	****Explanation**** : We get the maximum are by picking bars 7, 5 and 9 The area is computed (smallest height) * (no. of the picked bars) = 5 * 3 = 15

#### Solution : 
**Brute Approach** 
	consider every bar of histogram 
	for each bar go to the left and right to check for the smaller 
	main
	and also maintain a Global maximum to get ans 
	
**Little Optimised Approach**
	Build an array Previous smaller Next smaller  array for each point 
	 Apply the logic of next greater to find for previous and next also at the same time 
	 `width = nextS[i] –prevS[i] – 1.`
	 Area = width x height of the i th bar
	 You also have the ans that is there for to maintain the highest area 

