# Subtle Memory Management and Concurrency Bugs in Objective-C

This repository demonstrates two common, yet subtle, bugs in Objective-C related to memory management and concurrency.  The first showcases improper object retention/release leading to memory leaks or crashes. The second illustrates race conditions that can occur with nonatomic properties when accessed concurrently from multiple threads.

## Bug 1: Memory Management Issues
The `bug.m` file demonstrates a memory leak due to improper release of an object. The `bugSolution.m` demonstrates how to use ARC or manual retain/release to fix this. 

## Bug 2: Concurrency Issues
The `bug.m` file also demonstrates a race condition that can occur due to concurrent modification of nonatomic properties.
The `bugSolution.m` shows how to use synchronization mechanisms (e.g., locks or atomic properties) to resolve this issue.

## How to Run
Compile and run the provided Objective-C code using Xcode or a similar environment. Observe the behavior with and without the fixes.