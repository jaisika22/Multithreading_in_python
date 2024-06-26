# Multithreading_in_python

Demonstrating matrix multiplication with multithreading. It calculates the product of 100 random matrices of size 1000x1000 with a constant matrix of the same size using multiple threads. It also measures the time taken and CPU usage for different numbers of threads.

## Results Interpretation

Time Taken (Sec): Indicates the time taken for matrix multiplication in seconds. Lower values indicate better performance.
Number of Threads: The number of threads used for matrix multiplication. Higher values may improve performance up to a certain point, depending on the system's capabilities.
CPU Usage: Percentage of CPU being used.

## Result DataFrame

|index|Threads|Time Taken \(Sec\)|CPU Usage \(%\)|
|---|---|---|---|
|0|1|11\.526117086410522|9\.18|
|1|2|9\.042523622512817|11\.40|
|2|3|8\.412841320037842|6\.37|
|3|4|8\.664864778518677|11\.32|
|4|5|7\.110133647918701|10\.98|
|5|6|8\.55474591255188|12\.18|
|6|7|7\.338780164718628|12\.24|
|7|8|8\.44337010383606|11\.07|
|8|9|7\.245795249938965|11\.36|
|9|10|8\.629744291305542|10\.62|


### Graphical Results
### 1. Cores Utilization: 
A line plot showing CPU utilization over the course of matrix multiplication experiments. This visualization provides insights into how effectively CPU cores are utilized during multi-threaded computation tasks.

![image](https://github.com/jaisika22/Multithreading_in_python/assets/107528387/62a34c8a-b2e4-4b5b-a260-3f4dc2ef17dd)





### 2. CPU USUAGE vs Number of Threads:

![image](https://github.com/jaisika22/Multithreading_in_python/assets/107528387/d6326a5c-0fb8-41fe-8f67-fba738cbb055)


![image](https://github.com/jaisika22/Multithreading_in_python/assets/107528387/ac34c513-72f9-4979-bf2b-edc408695444)
![image](https://github.com/jaisika22/Multithreading_in_python/assets/107528387/504e321b-6b0a-4252-99dc-c817ed63b13d)


From the results obtained, we can draw the following conclusions:

1. As the number of threads increases, the time taken for matrix multiplication generally decreases, up to a certain point. Beyond that point, the overhead of thread creation and management may outweigh the benefits of parallelism.
2. CPU usage decreases as the number of threads increases, as expected but after a certain number of threads, it starts increasing. However, it's essential to note that the distribution of CPU usage across cores may vary depending on the system architecture and workload.
