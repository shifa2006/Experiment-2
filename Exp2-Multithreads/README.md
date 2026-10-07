# Multithreaded Programming Using Pthreads and OpenMP

## Overview

This experiment demonstrates multithreaded programming using Pthreads and OpenMP. The experiment covers thread creation, multiple threads, work distribution, race conditions, synchronization, barriers, and performance analysis.

The experiment also compares the execution performance of Pthreads and OpenMP using different numbers of threads.

---

## Problem Definition

A sequential program executes the complete computation using a single thread. Multithreading allows the workload to be divided among multiple threads so that different parts of the computation can execute concurrently.

The experiment demonstrates how threads are created and managed using Pthreads and OpenMP, how race conditions occur when shared data is accessed without synchronization, and how synchronization mechanisms can be used to obtain correct results.

The performance of Pthreads and OpenMP is measured using different thread counts and compared using execution time, speedup, and efficiency.

---

## Experiment Objective

The main objectives of this experiment are:

- To understand thread creation and management.
- To create and execute multiple threads using Pthreads.
- To divide work among multiple threads.
- To understand race conditions.
- To solve race conditions using synchronization.
- To understand OpenMP parallel regions.
- To perform work sharing using OpenMP.
- To understand critical sections and barriers.
- To measure execution time for different thread counts.
- To compare Pthreads and OpenMP performance.
- To calculate speedup and efficiency.

---

## Implementations

| Implementation | Purpose |
|---|---|
| `thread1.c` | Create and execute one thread |
| `thread2.c` | Create and execute multiple threads |
| `thread_sum.c` | Divide work among multiple threads |
| `race.c` | Demonstrate race condition |
| `mutex.c` | Solve race condition using mutex |
| `omp1.c` | Demonstrate OpenMP parallel region |
| `omp_sum.c` | Perform work sharing using OpenMP |
| `omp_race.c` | Demonstrate OpenMP race condition |
| `omp_critical.c` | Synchronize using OpenMP critical section |
| `omp_barrier.c` | Coordinate threads using OpenMP barrier |
| `sequential.c` | Sequential performance baseline |
| `pthread_perf.c` | Measure Pthreads performance |
| `omp_perf.c` | Measure OpenMP performance |

---

## Recorded Results

### Pthreads Basic Programs

The single-thread program produced:

![Single Thread Output](E:\PGC LAB\Exp2-Multithreads\Pthreads.png)

The multiple-thread program produced messages from four threads:

![Multiple Thread Output](pthreads/results/thread2.png)

The work distribution program produced:

![Work Distribution Output](pthreads/results/thread_sum.png)

### Pthreads Race Condition

The race-condition program produced:

![Race Condition Output](pthreads/results/race.png)

The actual value is different from the expected value because multiple threads update the shared variable without synchronization.

### Pthreads Mutex

After applying mutex synchronization:

![Mutex Output](pthreads/results/mutex.png)

This shows that the shared variable is updated correctly when access is synchronized.



