# Multithreading_in_python

Demonstrating matrix multiplication with multithreading. It calculates the product of 100 random matrices of size 1000x1000 with a constant matrix of the same size using multiple threads. It also measures the time taken and CPU usage for different numbers of threads.

## Results Interpretation

Time Taken (Sec): Indicates the time taken for matrix multiplication in seconds. Lower values indicate better performance.
Number of Threads: The number of threads used for matrix multiplication. Higher values may improve performance up to a certain point, depending on the system's capabilities.
CPU Usage: Percentage of CPU being used.

## Result DataFrame

|index|Threads|Time Taken \(Sec\)|CPU Usage \(%\)|
|---|---|---|---|
|0|1|0\.06374049186706543|11\.51|
|1|2|0\.06310033798217773|11\.07|
|2|3|0\.059578895568847656|11\.28|
|3|4|0\.06240510940551758|10\.91|
|4|5|0\.05831623077392578|6\.55|
|5|6|0\.13833165168762207|7\.58|
|6|7|0\.05970430374145508|10\.7|
|7|8|0\.06813549995422363|10\.93|
|8|9|0\.0591273307800293|11\.01|
|9|10|0\.06149554252624512|11\.02|   


### Graphical Results
### 1. Cores Utilization: 
A line plot showing CPU utilization over the course of matrix multiplication experiments. This visualization provides insights into how effectively CPU cores are utilized during multi-threaded computation tasks.

![image](https://github.com/jaisika22/Multithreading_in_python/assets/107528387/3a2f9075-e0e3-4275-abd5-b8706b691cb6)



### 2. CPU USUAGE vs Number of Threads:

![image](https://github.com/jaisika22/Multithreading_in_python/assets/107528387/31bd1867-f1ee-4d2a-973f-6150e4190f8b)
![image](https://github.com/jaisika22/Multithreading_in_python/assets/107528387/ac34c513-72f9-4979-bf2b-edc408695444)
![image](https://github.com/jaisika22/Multithreading_in_python/assets/107528387/504e321b-6b0a-4252-99dc-c817ed63b13d)


From the results obtained, we can draw the following conclusions:

1. As the number of threads increases, the time taken for matrix multiplication generally decreases, up to a certain point. Beyond that point, the overhead of thread creation and management may outweigh the benefits of parallelism.
2. CPU usage decreases as the number of threads increases, as expected. However, it's essential to note that the distribution of CPU usage across cores may vary depending on the system architecture and workload.
