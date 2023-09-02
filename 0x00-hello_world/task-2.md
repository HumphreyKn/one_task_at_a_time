# Question 2: Assembler
## Written by: Humphrey Kinoti
## Date: 2023-08-29

### Question
Write a script that generates the assembly code of a C code and saves it in a file.
  - The C file name will be saved in the variable `$CFILE`
  - The output file should be named the same as the C file, but with the extension `.s` instead of `.c`.
    - Example: if the C file is `main.c`, the output file should be `main.s`

### Explanation
    - The script is written in bash
    - The script takes in a C file as an argument
    - The C file is saved in the variable `$CFILE`
    - The script generates the assembly code of the C file
    - The output file is named the same as the C file but with the extension `.s` instead of `.c`
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
    - The compilation process in C

After the compiler has finished processing the C file, the assembler takes over. Here is what the assembler does:
    - The assembler generates an assembly file from the C file, with a `.s` extension
    - The assembler does not generate an object file
    - The assembler does not link the assembly file
    - The assembler does not generate an executable file
    - The assembler does not generate a shared library