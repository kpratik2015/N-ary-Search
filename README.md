# N-ary-Search

N-ary search code in C with comments. Implemented using OpenMP library.

## Concept 

Depending on cores of Computer (e.g. 4 cores for dual core), threads are generated which divide the array of numbers into smaller arrays assigned to each thread.
The array of numbers is sorted already so the threads check the upper and lower bound number of their small arrays. If the number lies between the bounds of a small array then that array's index is taken as starting point for next further division. This goes on until last set of array with same number of elements as number of threads remain and we find number in one of the thread's array location.
