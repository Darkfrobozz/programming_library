This part of memory follows a [[heap]] data structure.
It entails that it is less organized but also much more flexible as an allocation can come in any size at any time during execution and popping can also come at any time.

Accessing the heap memory at some point goes through [[stack_mem]] or other memory that is not allocated.

This works because pointers are of fixed size.

Because the heap is disorganized, it can be quite slow to access and to allocate on.

An example of heap allocation is when creating a variadic [[string]].