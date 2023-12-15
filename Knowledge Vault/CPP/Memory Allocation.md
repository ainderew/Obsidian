 
<span style="font-weight:900; font-size:2rem";>Stack</span>
Is a region of a computer's memory that operates in a last-in, first-out (LIFO) manner. It means that the last item added to the stack is the first one to be removed. The stack is used for storing function call information, local variables, and control flow data.

When a function is called, the function's parameters and local variables are pushed onto the stack. When the function finishes executing, the values on the stack are popped off, and the control flow returns to the calling function. This stack-based memory management is highly efficient but has limited size, and variables stored on the stack must have a fixed size known at compile-time. The stack is a reserved region of RAM used primarily for the program's execution flow and function call management. It stores things like function call information, local variables, and [[#^75bbbd|Control Flow Data]].

- **LIFO (Last-In, First-Out):** Data is added and removed from the stack in a Last-In, First-Out manner.
- Allocation and deallocation on the stack are faster compared to the heap because it simply involves moving the stack pointer.
- The size of the stack is usually limited, and it's determined at compile time.
- Variables allocated on the stack have a short lifetime and go out of scope when the function that created them exits.
- Arrays and structures with a fixed size are often allocated on the stack.


<span style="font-weight:900; font-size:2rem";>Heap</span>
The heap is a larger pool of memory used for dynamic memory allocation. It's a region of a computer's memory space where data can be allocated and deallocated in a non-linear order. Unlike the stack, the heap does not have a size limit (other than the system's physical memory) and is used for objects whose size is not known at compile-time, like data structures, arrays, or objects created during the program's runtime.


In languages like C and C++, developers use functions like `malloc()` and `free()` to allocate and deallocate memory on the heap manually. In languages like Java, Python, or C#, memory management for the heap is handled automatically by the runtime environment's garbage collector. This automatic memory management helps prevent issues like memory leaks (unreleased memory) and dangling pointers (pointers that reference deallocated memory locations).

- Data can be allocated and deallocated in any order.
- Allocation and deallocation on the heap are slower than the stack because it requires finding a block of unused memory of the appropriate size.
- The size of the heap is usually much larger than the stack, and it can grow and shrink during runtime.
- Variables allocated on the heap can have a longer lifetime than stack variables. They persist until explicitly deallocated.
- Objects and data structures of unknown size at compile time are allocated on the heap using functions like `malloc()` and `new` (in languages like C and C++)
- Dynamic data structures like linked lists, trees, and graphs are often implemented on the heap due to their variable and unpredictable size.


both the stack and the heap are parts of a computer's RAM. In many modern programming languages, there is also a concept of automatic memory management (garbage collection), which helps in managing memory on the heap efficiently, reducing the risk of memory leaks and dangling pointers.














<span style="font-weight:900; color:#57C8FD";>Related Terms</span>

**Control Flow Data:** Control flow data refers to the information necessary for the program to keep track of its execution sequence. This includes details such as the return address (the memory address to which the function should return after it completes its execution), the current program counter (the memory address of the next instruction to be executed), and other data related to function calls and branching within the program. ^75bbbd

For example, consider a simple function in C programming language:

```c
int addNumbers(int a, int b) {
    int result = a + b;
    return result;
}
```

When the `addNumbers` function is called, control flow data on the stack might look like this:

- **Return Address:** The memory address to which the program should return after the function completes. This is the address where the function call was made from.
- **Function Parameters:** In this case, the values of `a` and `b`.
- **Local Variables:** The space for the `result` variable.


**Function Call Information:** Function call information includes details about the functions being called, such as function parameters and return values. These details are crucial for managing function calls and ensuring that functions can operate with the correct data.

For example, consider a program that calculates the factorial of a number:

```c
int factorial(int n) {
    if (n == 0 || n == 1) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}
```

When the `factorial` function is called with a specific value of `n`, the function call information includes the value of `n` and the return value of the function call. The recursive nature of this function means that multiple instances of the function might be called, each with its own set of function call information on the stack.