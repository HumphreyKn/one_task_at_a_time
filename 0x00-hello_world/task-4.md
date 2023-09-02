# Question 4: Hello, puts
## Written by: Humphrey Kinoti

## Question
Write a C program that prints exactly `"Programming is like building a multilingual puzzle`, followed by a new line.

    - Use the function `puts`
    - You are not allowed to use `printf`
    - Your program should end with the value `0`

### Explanation
    - The program is written in C
    - The program prints the string `Programming is like building a multilingual puzzle`
    - The string is printed using the function `puts`
    - The program ends with the value `0`
    - The program will be compiled using the gcc compiler flags `-Wall -Werror -Wextra -pedantic -std=gnu89`

### What you need to know to complete the task
#### The gcc flags `-Wall -Werror -Wextra -pedantic -std=gnu89`.
We have previously learnt how to compile a C program using the gcc compiler. We will now learn how to compile a C program using the gcc compiler flags `-Wall -Werror -Wextra -pedantic -std=gnu89`. The flags are used to compile a C program in a specific way. 

**Remember: RTFM (Read The F\*\*\*ing Manual)** `man gcc`

##### The flag `-Wall`
The flag `-Wall` is used to enable all the warnings about constructions that some users consider questionable, and that are easy to avoid (or modify to prevent the warning), even in conjunction with macros. This enables many more warnings by default and is used to compile a C program in a specific way.

##### The flag `-Werror`
The flag `-Werror` is used to make all warnings into errors. This is used to compile a C program in a specific way. It treats all warnings as errors. The compiler will now stop compiling when it encounters a warning. 

##### The flag `-Wextra`
The flag `-Wextra` is used to enable some extra warning flags that are not enabled by `-Wall`. 

##### The flag `-pedantic`
The flag `-pedantic` is used to issue all the warnings demanded by strict ISO C and ISO C++.

##### The flag `-std=gnu89`
The flag `-std=gnu89` is used to compile a C program in a specific way. It specifies the language standard to be used. The value `gnu89` specifies the C language standard. The value `gnu89` is used to specify the C language standard because it is the default value.

#### The function `puts`
The function `puts` is used to print a string to the standard output (stdout). The function `puts` is defined in the header file `stdio.h`. The function `puts` returns a non-negative value on success and EOF on failure. The function `puts` is declared as follows:
```C
int puts(const char *str);
```
The function `puts` takes in a string as an argument. The string is passed to the function as a pointer to the first character of the string. 

**Remember: RTFM (Read The F\*\*\*ing Manual)** `man 3 puts`

#### The function `main`
The function `main` is the entry point of a C program. 

#### The return value of the function `main`
The function `main` returns an integer value. The return value of the function `main` is used to determine the exit status of the program. The exit status of a program is used by the operating system to determine whether the program executed successfully or not.

Whenever the return value of the function `main` is `0`, the program is said to have executed successfully. Whenever the return value of the function `main` is not `0`, the program is said to have failed to execute successfully.

*NB:* **Whenever the compiler encounters a return statement in any function in C, it stops executing the function and returns the value specified in the return statement.**

#### Special characters and escape sequences
Special characters are characters that are not printable. Special characters are represented using escape sequences. Escape sequences are sequences of characters that represent special characters. Escape sequences are used to represent special characters in a string.

The following are some of the special characters and their escape sequences:
| Special character | Escape sequence |
| ----------------- | --------------- |
| `"`               | `\"`            |
| `\`               | `\\`            |
| `\n`              | `\\n`           |
| `\t`              | `\\t`           |
| `\?`              | `\\?`           |
| '?'               | `\\x3f`         |
