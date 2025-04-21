# Compile Time vs Run Time

## Overview

| Aspect | Compile Time | Run Time |
|--------|--------------|-----------|
| When it happens | Before the program is run | While the program is running |
| Who handles it | Compiler | Operating System (during execution) |
| Main activities | Syntax checks, type checks, converting code to machine code | Executing code, handling user inputs, memory allocation |
| Errors | Compile-time errors (syntax errors, type mismatches) | Run-time errors (divide by zero, null reference, out of bounds) |

## Example

```cpp
#include <iostream>
using namespace std;

int main() {
    int x = "Hello";  // ❌ Compile-time error: assigning string to int
    cout << 10 / 0;   // ❌ Run-time error: division by zero
    return 0;
}
```

### What happens here:

**Compile Time:**
- The line `int x = "Hello";` will fail during compilation because "Hello" is a string and x is an int. This is a compile-time error.

**Run Time:**
- If you fix the above error and write `int x = 5;`, the program will compile, but when it reaches `10 / 0`, the program crashes while running because of a divide-by-zero error, which is a run-time error.

## One-Line Analogy
Compile time is when your program is getting ready to run (like checking your bags before a flight), and run time is when your program is actually running (you're on the flight and anything can happen).

# Compiled vs Interpreted Languages

## Overview

| Category | Compiled Language | Interpreted Language |
|----------|-------------------|----------------------|
| Examples | C, C++, Rust, Go, Swift | Python, JavaScript, Ruby |
| Compilation | Converts code to machine code before running | Executes code line-by-line |
| Speed | Generally faster | Generally slower |
| Error Detection | Many errors caught at compile time | Errors found during execution |
| Output | Binary/executable file | No separate binary, just the interpreter runs the code |

## Hybrid Languages
Some languages blur the line:
- **Java**: Compiled to bytecode, then interpreted (or JIT compiled)
- **JavaScript** (in browsers): Often JIT compiled now for speed
- **Python**: Can be compiled to bytecode (.pyc), but still interpreted

## Compiler vs Interpreter

### Compiler (for Compiled Languages)
A compiler is a tool that translates the entire source code of a program into machine code (or some intermediate code), before it runs.

✅ **Input**: Source code (.c, .cpp, .go)  
✅ **Output**: Executable (.exe, binary)  
✅ **When**: Happens before the program runs

#### Examples of Compilers:

| Language | Compiler |
|----------|----------|
| C | gcc (GNU Compiler Collection) |
| C++ | g++, clang |
| Go | Go Compiler (go build) |
| Rust | rustc |
| Swift | swiftc |

### Interpreter (for Interpreted Languages)
An interpreter reads and executes code line-by-line, without compiling the whole thing into a separate executable beforehand.

✅ **Input**: Source code (.py, .js)  
✅ **Output**: Nothing saved; just executed  
✅ **When**: Happens while the program is running

#### Examples of Interpreters:

| Language | Interpreter |
|----------|------------|
| Python | python, python3 |
| JavaScript | V8 (Chrome), SpiderMonkey (Firefox), JavaScriptCore (Safari) |
| Ruby | ruby |
| PHP | php |
| Bash | bash shell |

## Error Handling

### Compiled Languages (e.g., C++, Go, Rust)
- Error detection happens at compile time
- Syntax errors, type mismatches, missing declarations, etc., are caught before the code runs
- You cannot run the program unless it compiles successfully

**Example (C++):**
```cpp
int main() {
    int x = "hello"; // ❌ Compile-time error: invalid conversion
    return 0;
}
```
This won't even compile — the error must be fixed first.

### Interpreted Languages (e.g., Python, JavaScript)
- Error detection happens at run time
- Code is executed line-by-line, so errors are only caught when that line runs
- You can run the script, and it may work partially before it crashes

**Example (Python):**
```python
print("This will run")
x = "text" + 5  # ❌ Run-time TypeError
print("This will not run")  # never reached
```

### Error Handling Comparison

| Aspect | Compiled Language | Interpreted Language |
|--------|-------------------|----------------------|
| Error detection | At compile time | At run time |
| Execution halts? | Stops before running | Stops at the error line |
| Partial execution | ❌ Not possible | ✅ Possible before error occurs |
| Safety | Safer before deployment | More flexible during development |

## Summary Analogy
Imagine you're cooking from a recipe:
- **Compiled language** is like checking the entire recipe and verifying you have all ingredients before cooking
- **Interpreted language** is like starting to cook and only realizing you don't have salt when the recipe says "add salt"

