# Cuda-programming
Problem 1:
1.Write and compile an example of “Vector Add”  both for CPU and GPU. Use argument N as the length of the vectors. Compare to the performance of CPU and GPU over the increasing value of N (1K, 10K, 100K, 1M, and 10M). Measure the execution time for CPU and GPU and show that how the CPU and GPU performance and relative GPU over CPU speedup scale with increasing job size (N as the length of array). When measuring the performance only focus on the kernel execution time and ignore the time for transferring the data between CPU and GPU. Make sure to elaborate your result

2.For job size of 1M (N=1M), vary the thread block size (TB= 128, 256, 512, 1024). Plot and demonstrate how execution time of the kernel (offset the execution time for data transfer) varies over different thread block sizes. Plot your results. Make sure to elaborate your results.

3.plot the results for both 1.a and 1.b, this time consider the additional overhead of moving data between the host and device. Argue how the benefits of GPU accelerator changes when the overhead of data movement come to the picture. Make sure to elaborate your results.




Problem 2:
In this problem, we compile and run “1D Stencil” application on both CPU (single threaded) and GPU.
2.a Write and compile an example of “1D Stencil” similar to problem 1. Consider N as the job size (the length of array), and R as the radius of Stencil. Measure the speedup over CPU execution (with and without considering data movement between CPU and GPU) for increasing job size of N (1K, 10K, 100K, 1M, 10M), with the radius of 2 (R=2) and TB size=128. Plot your results including relative speed up with and without data movement. Make sure to elaborate your results.

2.b Compared the performance of CPU and GPU over the increasing value of N=10K, but R=2, 4, 8, 16. Focus on the kernels execution time, and plot the relative performance with TB size =128. Make sure to elaborate your results .

3.c Explore the opportunities for using the shared memory to enhance the performance benefits on GPUs. Demonstrate results that plot benefits/limitation of shared memory with respect to increasing job size (N), and radius size (R). consider TB size of 128 for all experiments. Make sure to elaborate your results and logically analyze your findings.
