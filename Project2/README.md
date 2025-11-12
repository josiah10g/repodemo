# Project2 - C Basics

This folder contains basic C files and examples.

## Basic C File Structure

### Hello World Example
Create a file named `hello.c`:
```c
// hello.c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

Compile and run:
```bash
gcc hello.c -o hello
./hello
```

### Basic C Concepts

#### Variables and Data Types
```c
// variables.c
#include <stdio.h>

int main() {
    int age = 25;              // Integer
    float height = 5.9;        // Float
    char grade = 'A';          // Character
    double pi = 3.14159;       // Double precision float
    
    printf("Age: %d\n", age);
    printf("Height: %.1f\n", height);
    printf("Grade: %c\n", grade);
    printf("Pi: %.5f\n", pi);
    
    return 0;
}
```

#### Functions
```c
// functions.c
#include <stdio.h>

// Function declaration
int add(int a, int b);

int main() {
    int result = add(5, 3);
    printf("Result: %d\n", result);
    return 0;
}

// Function definition
int add(int a, int b) {
    return a + b;
}
```

#### Arrays and Loops
```c
// arrays.c
#include <stdio.h>

int main() {
    int numbers[] = {1, 2, 3, 4, 5};
    int size = 5;
    
    // Loop through array
    for (int i = 0; i < size; i++) {
        printf("Number: %d\n", numbers[i]);
    }
    
    return 0;
}
```

#### Conditional Statements
```c
// conditionals.c
#include <stdio.h>

int main() {
    int age = 18;
    
    if (age >= 18) {
        printf("You are an adult\n");
    } else {
        printf("You are a minor\n");
    }
    
    return 0;
}
```

## Compiling and Running C Files

1. **Install GCC compiler**: 
   - Linux: `sudo apt-get install gcc`
   - macOS: Install Xcode Command Line Tools
   - Windows: Install MinGW or use WSL

2. **Compile a C file**: `gcc filename.c -o outputname`
3. **Run the compiled program**: `./outputname` (Linux/Mac) or `outputname.exe` (Windows)

## Common C File Extensions
- `.c` - C source files
- `.h` - C header files
- `.o` - Object files (compiled)
- `.out` - Executable output (default on Unix)

## Getting Started with C

1. **Install a C compiler**: GCC or Clang
2. **Choose an IDE**: VS Code, Code::Blocks, or CLion
3. **Learn the basics**: Variables, functions, pointers, and memory management
4. **Practice**: Start with simple programs and gradually increase complexity
