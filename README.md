# MLassignment1
numpy.mean() in Python
numpy.mean(arr, axis = None) : Compute the arithmetic mean (average) of the given data (array elements) along the specified axis
Parameters :
arr  : [array_like]input array. 
axis : [int or tuples of int]axis along which we want to calculate the arithmetic mean. Otherwise, it will consider arr to be flattened(works on all 
 the axis). axis = 0 means along the column and axis = 1 means working along the row. 
out  : [ndarray, optional]Different array in which we want to place the result. The array must have the same dimensions as expected output. 
dtype  : [data-type, optional]Type we desire while computing mean. 

Results : Arithmetic mean of the array (a scalar value if axis is none) or array with mean values along specified axis. 
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
