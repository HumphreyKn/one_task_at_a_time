# Question 5: Hello, printf
## Written by: Humphrey Kinoti

## Question
Write a C program that prints exactly `with proper grammar, but the outcome is a piece of art,`, followed by a new line.

    - Use the function `printf`
    - You are not allowed to use the function `puts`
    - Your program should return `0`
    - Your program should compile without warning when using the `-Wall gcc` option

### Explanation
    - The program is written in C
    - The program prints the string `with proper grammar, but the outcome is a piece of art,`
    - The string is printed using the function `printf`
    - The program ends with the value `0`
    - The program will be compiled using the gcc compiler flags `-Wall -Werror -Wextra -pedantic -std=gnu89`

### What you need to know to complete the task
Read the previous post on puts. This is just a continuation of the previous task. You will learn about the function `printf` in this task.

#### The function `printf`
The function `printf` is used to print a string to the standard output (stdout). The function `printf` is defined in the header file `stdio.h`. The function `printf` returns the number of characters printed on success and a negative value on failure. The function `printf` is declared as follows:
```C
int printf(const char *format, ...);
```
The function `printf` is a variadic function. A variadic function is a function that takes in a variable number of arguments. The function `printf` takes in a string as the first argument. The string is passed to the function as a pointer to the first character of the string. The string is called the format string. The format string is used to specify the format of the output. The format string can contain plain text and format specifiers. 
The format specifiers are used to specify the format of the output. The format specifiers are replaced by the values of the arguments passed to the function. The format specifiers are replaced by the values of the arguments passed to the function in the order in which they are passed. The format specifiers are preceded by the character `%`. The format specifiers are followed by a character that specifies the data type of the argument.

**Remember: RTFM (Read The F\*\*\*ing Manual)** `man 3 printf`

#### Format specifiers
Format specifiers define the type of data to be printed on the standard output (stdout). Some of the format specifiers are listed below:
| Format specifier | Data type                    |
|------------------|------------------------------|
| `%c`             | char                         |
| `%d`             | int                          |
| `%i`             | decimal integer              |
| `%u`             | unsigned int                 |
| `%o`             | octal number                 |
| `%x`             | hexadecimal number           |
| `%X`             | hexadecimal number           |
| `%s`             | string                       |
| `%p`             | pointer address              |
| `%f`             | float                        |
| `%e`             | scientific notation          |
| `%E`             | scientific notation          |
| `%g`             | shortest of `%e` and `%f`    |
| `%G`             | shortest of `%E` and `%f`    |
| `%%`             | `%`                          |
| `%n`             | number of characters printed |
| `%b`             | binary number                |
| `%hi`            | short (signed)               |
| `%hu`            | short (unsigned)             |
| `%li`            | long (signed)                |
| `%lu`            | long (unsigned)              |
| `%Lf`            | long double                  |