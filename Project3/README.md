# Project3 - C++ Basics

This folder contains basic C++ files and examples.

## Basic C++ File Structure

### Hello World Example
Create a file named `hello.cpp`:
```cpp
// hello.cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
```

Compile and run:
```bash
g++ hello.cpp -o hello
./hello
```

### Basic C++ Concepts

#### Variables and Data Types
```cpp
// variables.cpp
#include <iostream>
#include <string>

int main() {
    int age = 25;                    // Integer
    float height = 5.9;              // Float
    char grade = 'A';                // Character
    double pi = 3.14159;             // Double precision float
    std::string name = "John";       // String (C++ string class)
    bool is_student = true;          // Boolean
    
    std::cout << "Name: " << name << std::endl;
    std::cout << "Age: " << age << std::endl;
    std::cout << "Height: " << height << std::endl;
    std::cout << "Grade: " << grade << std::endl;
    
    return 0;
}
```

#### Functions
```cpp
// functions.cpp
#include <iostream>

// Function declaration
int add(int a, int b);

int main() {
    int result = add(5, 3);
    std::cout << "Result: " << result << std::endl;
    return 0;
}

// Function definition
int add(int a, int b) {
    return a + b;
}
```

#### Classes and Objects (OOP)
```cpp
// classes.cpp
#include <iostream>
#include <string>

class Person {
private:
    std::string name;
    int age;

public:
    // Constructor
    Person(std::string n, int a) : name(n), age(a) {}
    
    // Method
    void introduce() {
        std::cout << "Hi, I'm " << name << " and I'm " << age << " years old." << std::endl;
    }
};

int main() {
    Person person1("Alice", 25);
    person1.introduce();
    return 0;
}
```

#### Vectors and Loops
```cpp
// vectors.cpp
#include <iostream>
#include <vector>

int main() {
    std::vector<int> numbers = {1, 2, 3, 4, 5};
    
    // Loop through vector
    for (int num : numbers) {
        std::cout << "Number: " << num << std::endl;
    }
    
    return 0;
}
```

#### Conditional Statements
```cpp
// conditionals.cpp
#include <iostream>

int main() {
    int age = 18;
    
    if (age >= 18) {
        std::cout << "You are an adult" << std::endl;
    } else {
        std::cout << "You are a minor" << std::endl;
    }
    
    return 0;
}
```

## Compiling and Running C++ Files

1. **Install G++ compiler**: 
   - Linux: `sudo apt-get install g++`
   - macOS: Install Xcode Command Line Tools
   - Windows: Install MinGW or use WSL

2. **Compile a C++ file**: `g++ filename.cpp -o outputname`
3. **With C++11 or later**: `g++ -std=c++11 filename.cpp -o outputname`
4. **Run the compiled program**: `./outputname` (Linux/Mac) or `outputname.exe` (Windows)

## Common C++ File Extensions
- `.cpp` - C++ source files
- `.hpp` or `.h` - C++ header files
- `.cc` or `.cxx` - Alternative C++ source extensions
- `.o` - Object files (compiled)

## Getting Started with C++

1. **Install a C++ compiler**: G++ or Clang
2. **Choose an IDE**: VS Code, CLion, or Visual Studio
3. **Learn the basics**: Variables, functions, OOP (classes and objects), STL
4. **Practice**: Build small projects to understand the language features
5. **Explore STL**: Standard Template Library for containers and algorithms
