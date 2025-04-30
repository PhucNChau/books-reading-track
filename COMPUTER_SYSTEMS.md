# Computer Systems: A Programmer’s Perspective
[Back](/README.md)

__Keywords about the book__
- C programming language
- Assembly language, GCC compiler
- Computer organization
- Program performance
- Pipelining
- Processes, thread
- Virtual memory
- Concurrent Programming

## Contents
> [!Tip]
> Hover link to see page left of that chapter

Chap | Title | Link
---- | ---- | ----
1 | Overview | None
5 | Optimizing Program Performance | [read-5]
6 | The Memory Hierarchy | [read-6]

## Chapter 5
<!-- Change page number after reading to update -->
[read-5]: /COMPUTER_SYSTEMS.md#chapter-5 "480"
[Back to contents](/COMPUTER_SYSTEMS.md#contents)

### 5.1
Invoking _GCC_ with the command line flag '-O1' will cause it to apply a basic set of optimizations. Flag '-O2' or '-O3' applies more extensive application. But we only apply flag '-O1' to optimize C program by code.

_Optimization blockers_: aspects of programs that can severely limit the opportunities for a compiler to generate optimized code. There are two blockers:
* memory aliasing: The case where two pointers may designate the same memory location
* function calls and the function has _side effect_ - it modifies some part of the global program state.

### 5.2
The metric _cycles per element_, abbreviated “CPE,” is a way to express program performance


## Chapter 6
<!-- Change page number after reading to update -->
[read-6]: /COMPUTER_SYSTEMS.md#chapter-6 "596"
[Back to contents](/COMPUTER_SYSTEMS.md#contents)

### 6.1 Locality
Well-written computer programs -> exhibit good _locality_. That is:
* reference data items that are near other recently referenced data items
* or that were recently referenced themselves

Two distinct forms: _temporal locality_ and _spatial locality_.
* temporal locality: a memory location that is referenced once is likely to be referenced again multiple times in the near future
* spatial locality: if a memory location is referenced once, then the program is likely to reference a nearby memory location in the near future



