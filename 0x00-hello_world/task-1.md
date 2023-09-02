# Question 1: Compiler
## Written by: Humphrey Kinoti
## Date: 2023-08-29

## Question
Write a script that compiles a C file but does not link.
  - The C file name will be saved in the variable `$CFILE`
  - The output file should be named the same as the C file, but with the extension `.o` instead of `.c`.
    - Example: if the C file is `main.c`, the output file should be `main.o`

### Explanation
  - The script is written in bash
  - The script takes in a C file as an argument
  - The C file is saved in the variable `$CFILE`
  - The script compiles the C file but does not link it
  - The output file is named the same as the C file but with the extension `.o` instead of `.c`
  - The output file is saved in the current directory
  - The output file is created in the current directory

#### What you need to know to complete the task
Go through the previous task to learn about the following:
  - Bash Scripting
  - Variables
  - Special Variables
  - Rules for naming variables in bash
  - How to access variables in bash
  - How to declare variables in bash
  - How to assign values to variables in bash
  - The copilation process in C

After the preprocessor has finished processing the C file, the compiler takes over. Here is what the compiler does:
  - The compiler checks the syntax of the C file
  - The compiler checks for errors in the C file
  - The compiler generates an object file from the C file, with a `.o` extension
  - The compiler does not link the object file
  - The compiler does not generate an executable file
  - The compiler does not generate a shared library

### How to test the script
  - Create a file called `main.c` in the current directory
  - Add the following code to the file:
```c
#include <stdio.h>

int main(void)
{
    printf("Hello, World!\n");
    return (0);
}
```
  - Run the script with the following command:
```
./compiler
```
  - The output file should be named `main.o`
  - The output file should be saved in the current directory
  - The output file should be created in the current directory
  - The output file should be an object file
  - The output file should be created by the compiler

