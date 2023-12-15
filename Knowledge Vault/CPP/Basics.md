
- Compiling code
```bash
g++ -o myprogram main.cpp
```

- Making a header file
```c++
#ifndef PLAYER.H
#define PLAYER.H

// Header file contents go here  

#endif
```


- ### When to pass a pointer vs a reference
	The difference between pass-by-reference and pass-by-pointer is that pointers can be NULL or reassigned whereas references cannot. **Use pass-by-pointer if NULL is a valid parameter value or if you want to reassign the pointer**