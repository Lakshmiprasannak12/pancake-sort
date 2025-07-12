# Pancake-sort-using-python

*important points in pancake sort
1.high value
2.high value flip
3.total flip
4.set high value

example1:
8 2 7 5 1 3 9 4  
Flip at 7:[9, 3, 1, 5, 7, 2, 8, 4]
Flip at 8: [4, 8, 2, 7, 5, 1, 3, 9]
Flip at 2:[8, 4, 2, 7, 5, 1, 3, 9]
Flip at 7: [3, 1, 5, 7, 2, 4, 8, 9]
Flip at 4:[7, 5, 1, 3, 2, 4, 8, 9]
Flip at 6: [4, 2, 3, 1, 5, 7, 8, 9]
Flip at 4: [1, 3, 2, 4, 5, 7, 8, 9]
Flip at 2:[3, 1, 2, 4, 5, 7, 8, 9]
Flip at 3: [2, 1, 3, 4, 5, 7, 8, 9]
Flip at 2: [1, 2, 3, 4, 5, 7, 8, 9]

example2:

8 2 1 3 2 4 6 7 6
Flip at 9: [6, 7, 6, 4, 2, 3, 1, 2, 8]
Flip at 2:[7, 6, 6, 4, 2, 3, 1, 2, 8]
Flip at 8: [2, 1, 3, 2, 4, 6, 6, 7, 8]
Flip at 6:[6, 4, 2, 3, 1, 2, 6, 7, 8]
Flip at 7: [6, 2, 1, 3, 2, 4, 6, 7, 8]
Flip at 6: [4, 2, 3, 1, 2, 6, 6, 7, 8]
Flip at 5: [2, 1, 3, 2, 4, 6, 6, 7, 8]
Flip at 3:[3, 1, 2, 2, 4, 6, 6, 7, 8]
Flip at 4: [2, 2, 1, 3, 4, 6, 6, 7, 8]
Flip at 3: [1, 2, 2, 3, 4, 6, 6, 7, 8]

******Algorithm******
1.start with complete array and decrease the size of arr (n-1)
2.For each size  :
a.find index of max element from unsorted portion
b.flip the array with max element index value
c.for each size flip the total array to the current size
max->move to the end of the array
3.repeat step1 by n-2,n-3....
for nth reduced elemet perform step2 untill 0th index value respectively..
'''
