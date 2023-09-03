# Question 6: Size is not grandeur, and territory does not make a nation
## Written by: Humphrey Kinoti

## Question
Write a C program that prints the size of various types on the computer it is compiled and run on.

    - You should produce the exact same output as in the example
    - Warnings are allowed
    - Your program should return `0`
    - You might have to install the package `libc6-dev-i386` on your Linux to test the `-m32` gcc option
    - You are not allowed to use the `sizeof` operator

The C code is saved in the file `size.c`. The aim of this task is to learn the size of data types in C in different architectures, in this case a 64 bit architecture and a 32 bit architecture.

**Example:**
```bash
gcc size.c -m32 -o size32 2> /tmp/32 # compile with -m32 option
./size32 2> /tmp/322 # run with -m32 option
gcc size.c -m64 -o size64 2> /tmp/64 # compile with -m64 option
./size64 2> /tmp/642 # run with -m64 option
```
**Output:**
```bash
$ cat /tmp/32
Size of a char: 1 byte(s)
Size of an int: 4 byte(s)
Size of a long int: 4 byte(s)
Size of a long long int: 8 byte(s)
Size of a float: 4 byte(s)

$ cat /tmp/64
Size of a char: 1 byte(s)
Size of an int: 4 byte(s)
Size of a long int: 8 byte(s)
Size of a long long int: 8 byte(s)
Size of a float: 4 byte(s)
```
### Explanation
    - The program is written in C
    - The program prints the size of various types
    - The program prints the size of a char
    - The program prints the size of an int
    - The program prints the size of a long int
    - The program prints the size of a long long int
    - The program prints the size of a float
    - The program ends with the value `0`
    - Warnings are allowed, meaning we will not use the `-Werror` gcc option
    - Installing the package `libc6-dev-i386` on your Linux is required to test the `-m32` gcc option. If you are using Ubuntu, you can install the package `libc6-dev-i386` by running the command `sudo apt-get install libc6-dev-i386`
    - The exit status of the program should be `0`. This means that the program should execute successfully

### What you need to know to complete the task
#### The gcc flags `-m32` and `-m64`
We have previously learnt how to compile a C program using the gcc compiler. We will now learn how to compile a C program using the gcc compiler flags `-m32` and `-m64`. The flags are used to compile a C program in a specific way.

**Remember: RTFM (Read The F\*\*\*ing Manual)** `man gcc`
##### The flag `-m32`
The flag `-m32` specifies the architecture to be used. In this case, the architecture is `32-bit`. The flag `-m32` is used to compile a C program to be executed on a `32-bit` architecture because it is the default value.

##### The flag `-m64`
The flag `-m64` specifies the architecture to be used. In this case, the architecture is `64-bit`. The flag `-m64` is used to compile a C program to be executed on a `64-bit` architecture.

#### The `sizeof` operator
The `sizeof` operator is used to determine the size of a data type in bytes. The `sizeof` operator is a unary operator. A unary operator is an operator that takes in a single operand. The `sizeof` operator is used as follows:
```C
sizeof (data_type)
```
The `sizeof` operator takes in a data type as an argument. The data type is passed to the `sizeof` operator as a type name. The `sizeof` operator returns the size of the data type in bytes. 
