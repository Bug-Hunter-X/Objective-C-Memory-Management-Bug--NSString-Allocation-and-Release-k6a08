# Objective-C Memory Management Bug: NSString Allocation and Release

This repository demonstrates a common error in Objective-C related to memory management. Specifically, it highlights a potential memory leak that can occur when allocating an NSString without properly releasing it using the appropriate method. 

The `bug.m` file contains the erroneous code, while `bugSolution.m` provides the corrected version. The core issue involves how to manage the lifecycle of the NSString object to prevent resource leaks.

## How to reproduce the bug:

1. Compile and run `bug.m`.
2. Observe that, while it does not immediately crash, it does not properly release the memory associated with the allocated NSString.

## Solution:

The solution provided in `bugSolution.m` addresses the problem by correctly managing the object's lifecycle. The primary change is the handling of memory management (in this case, ensuring that memory is deallocated when no longer needed).