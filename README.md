# S22_15618_Project
This is the final project for CMU 15618 course.

andrewid: 
xuelinz
shanyuew

# Proposal
## Summary
In this project, we are going to investigate the performance of the apple newly produced ARM based architecture chip M1 max. Specifically, we are going to divide the project into two perspective. Firstly, we are going to investigate the M1 max performance in SIMD applications. Secondly, we are also intereseted in the design and performance of neural engines on M1 max.

## Background
M1 max chip is apple's newly produced chip based on ARM. The newly produced chip has become super popular due to its performance in the desktop's chip. Also, ARM architecture made a breakthrough in the nowdays' x86 dominated desktop chip market. In this project, we are going to investigate the chip in details and understand two aspects, SIMD on ARMS and M1 max neural engine performance.

## Challenges
**Parallelism perspective:**
We are going to investigate the SIMD performance of ARM based chip and x86 chip. Studying from the instruction level, we are going to answer questions like: does this arm chip have  fixed-length vectors, support scatter-gather and support permutations?

**Computer architecture perspective:**
Besides, we are going to investigate the nearul engine performance. We are going to divise a way to accurately benchmarking the performances of M1 chips and x86 chips. Also, we intend to compare the performance with GPU. Derived from the benchmark results, we are going to understand the architecture reasons behind the hood, which leads to the performance boost or degradation.

## Resources
Local computer 2021 MacBook Pro (Apple M1 Max with 10-core CPU, 24-core GPU, 16-core Neural Engine), 2019 MacBook Pro with Intel chip (8-core Intel Core i7-9750H).

Ghc NVIDIA GPU (NVIDIA GeForce RTX 2080 B GPU).

## Goals and deliverables
### 75% goal
Write a benchmark program to compare the SIMD performance of an Intel chip and an M1 max chip. Analye features affecting the SIMD performance of a chip.
### 100% goal
Explore M1 max chip SIMD instruction set and compare its supported features against an Intel chip.
### 125% goal
Explore M1 max chip's nerual engine unit, benchmark its performance and explain what designs makes it possible to speedup deep learning tasks.

## Schedule
03/27/2022 Explore common benchmark problems and choose one.

04/02/2022 Implment the benchmark program on both platforms.

04/09/2022 Perform benchmark experiments and identify features affecting a CPU's SIMD performance.

04/16/2022 Analysis extra SIMD features supported by M1 max, such as catter-gather and permutations.

04/30/2022 Benchmark common AI jobs on M1 max, describe their computation patterns and explain why can nerual engine accelerate these computation patterns.

# Diliverables
Please find the report in the same directory. `final_report.pdf`

Here are some important benchmark figures.

# CPU

![image](imgs/Geekbench%20Single-Core%20Score.png)

![image](imgs/Geekbench%20Multi-Core%20Score.png)

![image](imgs/Geekbench%20Multi-Core%20Speedup.png)


# GPU
![image](imgs/gpu_inference.jpg)

![image](imgs/gpu_training.jpg)

# ANE
![image](imgs/neural_benchmark.jpg)