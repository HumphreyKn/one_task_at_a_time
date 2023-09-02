# Question 3: Name
## Written by: Humphrey Kinoti

## Question
Write a script that compiles a C file and creates an executable named `cisfun`.
  - The C file name will be saved in the variable `$CFILE`

### Explanation
    - The script is written in bash
    - The script takes in a C file as an argument
    - The C file is saved in the variable `$CFILE`
    - The script compiles the C file
    - The script creates an executable named `cisfun`
    - The executable is saved in the current directory
    - The executable is created in the current directory

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

It ia possible to save the executable in a file name of your choice. To do this, you need to pass the `-o` flag to the compiler. Here is an example:
```C
gcc main.c -o my_executable
```
The above command will create an executable named `my_executable` in the current directory. By default, the executable is named `a.out` (if the executable name is not specified).