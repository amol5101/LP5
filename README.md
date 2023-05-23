# LP5
DFS O/P

node = 4, edges = 6  ,start node=0 

0 -> 1, 0 -> 2, 1 -> 2, 2 -> 0, 2 -> 3, 3 -> 3 

0 2 3 1

node = 4, edges = 6  ,start node=2

2 -> 0, 0 -> 2, 1 -> 2, 0 -> 1, 3 -> 3, 1 -> 3 

2 1 3 0

How Parallel Bubble Sort Work

● Parallel Bubble Sort is a modification of the classic Bubble Sort algorithm that takes advantage of

parallel processing to speed up the sorting process.

● In parallel Bubble Sort, the list of elements is divided into multiple sublists that are sorted

concurrently by multiple threads. Each thread sorts its sublist using the regular Bubble Sort

algorithm. When all sublists have been sorted, they are merged together to form the final sorted

list.

● The parallelization of the algorithm is achieved using OpenMP, a programming API that supports

parallel processing in C++, Fortran, and other programming languages. OpenMP provides a set of

compiler directives that allow developers to specify which parts of the code can be executed in

parallel.

● In the parallel Bubble Sort algorithm, the main loop that iterates over the list of elements is

divided into multiple iterations that are executed concurrently by multiple threads. Each thread

sorts a subset of the list, and the threads synchronize their work at the end of each iteration to

ensure that the elements are properly ordered.

● Parallel Bubble Sort can provide a significant speedup over the regular Bubble Sort algorithm,

especially when sorting large datasets on multi-core processors. However, the speedup is limited

by the overhead of thread creation and synchronization, and it may not be worth the effort for

small datasets or when using a single-core processor.


How Parallel Merge Sort Work

● Parallel merge sort is a parallelized version of the merge sort algorithm that takes advantage of

multiple processors or cores to improve its performance. In parallel merge sort, the input array is

divided into smaller subarrays, which are sorted in parallel using multiple processors or cores.

The sorted subarrays are then merged together in parallel to produce the final sorted output.

● The parallel merge sort algorithm can be broken down into the following steps:


● Divide the input array into smaller subarrays.

● Assign each subarray to a separate processor or core for sorting.

● Sort each subarray in parallel using the merge sort algorithm.

● Merge the sorted subarrays together in parallel to produce the final sorted output.

● The merging step in parallel merge sort is performed in a similar way to the merging step in the

sequential merge sort algorithm. However, because the subarrays are sorted in parallel, the

merging step can also be performed in parallel using multiple processors or cores. This can

significantly reduce the time required to merge the sorted subarrays and produce the final output.

● Parallel merge sort can provide significant performance benefits for large input arrays with many

elements, especially when running on hardware with multiple processors or cores. However, it

also requires additional overhead to manage the parallelization, and may not always provide

performance improvements for smaller input sizes or when run on hardware with limited parallel

processing capabilit
