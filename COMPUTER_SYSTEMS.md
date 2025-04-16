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
5 | Optimizing Program Performance | [read]

## Chapter 5
<!-- Change page number after reading to update -->
[read]: /COMPUTER_SYSTEMS.md#chapter-5 "480"
[Back to contents](/COMPUTER_SYSTEMS.md#contents)

### 5.1
Invoking _GCC_ with the command line flag '-O1' will cause it to apply a basic set of optimizations. Flag '-O2' or '-O3' applies more extensive application. But we only apply flag '-O1' to optimize C program by code.

_Optimization blockers_: aspects of programs that can severely limit the opportunities for a compiler to generate optimized code. There are two blockers:
* memory aliasing: The case where two pointers may designate the same memory location
* function calls and the function has _side effect_ - it modifies some part of the global program state.

### 5.2
The metric _cycles per element_, abbreviated “CPE,” is a way to express program performance


