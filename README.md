# MLassignment1
assignment1 IIT B 
# Python Program illustrating 
# numpy.mean() method   
import numpy as np
  

# 2D array 
arr = [[14, 17, 12, 33, 44],  
       [15, 6, 27, 8, 19], 
       [23, 2, 54, 1, 4, ]] 
  
# mean of the flattened array 
print("\nmean of arr, axis = None : ", np.mean(arr)) 
  
# mean along the axis = 0 
print("\nmean of arr, axis = 0 : ", np.mean(arr, axis = 0)) 
 
# mean along the axis = 1 
print("\nmean of arr, axis = 1 : ", np.mean(arr, axis = 1))

out_arr = np.arange(3)
print("\nout_arr : ", out_arr) 
print("mean of arr, axis = 1 : ", 
      np.mean(arr, axis = 1, out = out_arr))
#Output :
mean of arr, axis = None :  18.6

mean of arr, axis = 0 :  [17.33333333  8.33333333 31.         14.         22.33333333]

mean of arr, axis = 1 :  [24.  15.  16.8]

out_arr :  [0 1 2]
mean of arr, axis = 1 :  [24 15 16]
