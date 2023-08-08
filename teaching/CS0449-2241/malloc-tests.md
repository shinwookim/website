---
layout: post
title: "Malloc Project: Writing Custom Test Cases (Traces)"
subtitle: "CS 0449: Introduction to System Software"
---
Testing software while developing is a crucial and indispensable aspect of the software development process. For this project, you are provided a set of *traces* (found in the `traces/` directory) that is used to test your `mm.c` implementation for correctness, space utilization, and throughput. Each *trace file* contains a sequence of allocate and free instructions that direct the driver program (`mdriver.c`) to call your `mm_malloc()` and `mm_free()` functions in some order{%sidenote "grading" "The provided driver and trace files are the same ones we will use when we grade your handin `mm.c` file, although we may change the order in which the traces are used."%}.

However, throughout the development of your malloc implementation, you may find it beneficial to write your own custom *trace files* (especially since the provided ones can get rather long). Doing so will (hopefully) help you better understand how the other trace files and the driver program operate.

## Creating a New Trace File
To write our custom trace, make a copy of the trace `short1-bal.rep`{%sidenote "start-trace" "The trace `short1-bal.rep` can be found in the `traces/` directory of the project."%} and rename it to `custom-trace.rep`{%sidenote "extension" "A trace file technically does not need to use the `.rep` file extension to be recognized by the driver program. However, it is often wise to follow pre-existing conventions for file names (and also function/variables names, etc.) of your project."%}.

By this point, you should have a trace file named `custom-trace.rep` in the `traces/` directory whose contents look something like:
```c
20000
6
12
1
a 0 2040
a 1 2040
/* ... */
f 4
f 5
```
## Modifying the Trace File
### Line 1: `20000` (Suggested Heap Size - Unused)
The first line in your trace file  sets a variable in driver program called the *suggested heap size* (`sugg_heapsize`). However, it turns out this variable is not actually used and we can ignore it. (**This  line, however, must still exists in the trace file**)

### Line 2: `6` (Number of Allocation IDs)
The next line denotes the number of allocation IDs. In essence, it is asking how many different blocks the trace file will allocate.

### Line 3: `12` (Number of Operations)
The third line denotes the number of total operations performed by the trace file. This number should be equal to the number of allocations + number of frees that appear in remained the trace file.

### Line 4: `1` (Weight of Trace - Unused)
Before the sequence of allocates (`a`) and frees(`f`) begins, the fourth line of the trace file denotes the weight of trace. However, much like the first line, this parameter is not used and can be ignored. (**This  line, however, must still exists in the trace file**)

### Line 5 - N: Allocations and Frees
The remainder of the trace file should contain the sequence of allocations and frees. A allocation is denoted using the `a` keyword and is written like:
```c
a 0 16
``` 
to instruct the driver to allocate `16` bytes and assign the resulting pointer to ID `0`. Similarly, a free is denoted using the `f` keyword and is written like:
```c
f 0
```
to instruct the driver to free the pointer with ID `0`.

Be sure to free all blocks before reaching the end of the trace and only free blocks that have already been allocated.

## Summary
```
1024100       /* Unused number */
12000         /* Number of IDs (how many allocations?) */
16000         /* Number of operations (# of allocation + # of free) */
1             /* Unused number */
a 0 16        /* allocate 16 bytes. Job ID = 0 */
a 1 112       /* allocate 112 bytes. Job ID = 1 */
(...)
```