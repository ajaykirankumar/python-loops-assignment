# python-loops-assignment

import numpy as np
import time
temps_celsius = np.array([22, 25, 28, 24, 26])
temps_fahrenheit = temps_celsius * 1.8 +32
avg_fahrenheit = np.round(np.mean(temps_fahrenheit), decimals=1)

print("Task 1 Output: ")
print("Celsius: ", temps_celsius)
print("Fahrenheit: ", temps_fahrenheit)
print("Average Fahrenheit: ",  avg_fahrenheit)

scores=np.array([85, 90, 78, 92, 88, 76, 95, 82, 89, 91, 87, 84])
print("\n Task 2 Output: ")
print("shape: " , scores.shape)
print("Total elements: ", scores.size)
print("Highest score: ", np.max(scores))
print("Lowest score: ", np.min(scores))
print("Range: ", np.max(scores) - np.min(scores))


numpy_array= np.arange(1, 50001)
python_list= list(range(1, 50001))
start_numpy = time.time()
numpy_sum = np.sum(numpy_array)
end_numpy = time.time()
numpy_time = end_numpy - start_numpy

start_python=time.time()
python_sum= sum(python_list)
end_python=time.time()
python_time = end_python - start_python
speed_difference = python_time / numpy_time

print("\n Task 3 Output: ")
print("Numpy Sum: ", numpy_sum)
print("python Sum: ", python_sum)
print("Numpy Time: {:.4f} seconds". format(numpy_time))
print("python Time: {:.4f} seconds". format(python_time))
print("Numpy is {:.1f}*faster". format(speed_difference))
