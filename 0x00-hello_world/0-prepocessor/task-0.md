# Question: 0. Preprocessor
## Written by: Humphrey Kinoti
## Date: 2023-08-29

### Question
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

### What you need to know to complete the task
#### Bash Scripting
Bash scripting is a way to interact with the computer using text commands. Scripts are used to run a series of commands. Bash is available by default on Linux and macOS operating systems. 

#### Variables
Variables are used to store data. Variables can be used to store strings, numbers, and other types of data. Variables are declared by assigning a value to them. Variables can be declared in the following ways:
  - `variable_name=value`
  - `variable_name="value"`

#### Special Variables
Special variables are variables that are set by the shell. They are used to get information about the shell and its environment. They are also used to get information about the last command that was run. Special variables are declared in the following ways:
  - `$?` - The exit status of the last command that was run
  - `$0` - The name of the shell or script
  - `$1` - The first argument passed to the script
  - `$2` - The second argument passed to the script
  - `$#` - The number of arguments passed to the script
  - `$@` - All the arguments passed to the script
  - `$*` - All the arguments passed to the script as a single string
  - `$$` - The process ID of the current shell
  - `$!` - The process ID of the last command that was run in the background
  - `$-` - The current options set for the shell
  - `$IFS` - The internal field separator
  - `$?` - The exit status of the last command that was run
  - `$LINENO` - The current line number in the script
  - `$RANDOM` - A random number between 0 and 32767
  - `$SECONDS` - The number of seconds since the shell was started
  - `$EUID` - The effective user ID of the current user
  - `$UID` - The real user ID of the current user

Rules for naming variables in bash:
  - Variables names must start with a letter or an underscore
  - Variable names can only contain letters, numbers, and underscores
  - Variable names cannot contain spaces
  - Variable names cannot start with a number
  - Variable names cannot contain special characters
  - Variable names cannot be the same as a keyword
  - There is no space between the variable name and the equal sign, and there is no space between the equal sign and the value

Variables can be accessed by using the `$` sign before the variable name. Variables can be accessed in the following ways:
  - `$variable_name`
  - `${variable_name}`
  - `$variable_name[index]`
  - `${variable_name[index]}`
  - `$variable_name[start:end]`
  - `${variable_name:start:end}`
  - `$variable_name[start:end:step]`
  - `${variable_name:start:end:step}`

#### shebang
A shebang, also known as a hashbang or pound-bang, is a special character sequence at the beginning of a script file that specifies the interpreter that should be used to execute the script. It is denoted by the characters `#!` followed by the path to the interpreter.
For example, if the script is written in bash, the shebang would be `#!/bin/bash`.

Here are a few key points about shebangs:
  - **Interpreter Specification:** The shebang line is used to specify the interpreter for the script. It should immediately follow the `#!` characters and include the path to the interpreter binary.
  - **Whitespace:** There should be no spaces or tabs between `#!` and the interpreter path. It must be a single line with no leading whitespace.
  - **Arguments:** The shebang line can include arguments to the interpreter. These arguments are separated from the interpreter path by a space.
  - **Multiple Arguments:** If there are multiple arguments, they should be separated by spaces.
  - **Quoting:** If the interpreter path or arguments contain spaces, they should be quoted.
  - **Comments:** Although not required, it's common practice to include a comment on the same line after the interpreter path to provide additional information or documentation about the script.
  - **Linux/Unix Convention:** Shebangs are primarily used in Linux and Unix-like operating systems to indicate the interpreter for shell scripts, Python scripts, Perl scripts, and more.
  - **Windows:** Shebangs are not used in Windows operating systems. Instead, the file extension (e.g., `.bat`, `.ps1`) is used to determine the interpreter for a script.
  - **Permission:** To execute a script with a shebang, you'll also need to ensure that the script file has the execute permission (e.g., `chmod +x script.sh`).

### The C compiling process
The C compiling process is a multi-step process that involves preprocessing, compiling, assembling, and linking. The C compiler is responsible for performing all of these steps. The C compiler is a program that takes C source code as input and produces an executable program as output. The C compiler is usually called `gcc` or `clang`. The C compiler is usually installed by default on Linux and macOS operating systems. The C compiler can be installed on Windows operating systems by installing the GNU Compiler Collection (GCC).
  - **preprocessing**
    - The C compiler first preprocesses the source code. This involves expanding macros, removing comments, and replacing header files with their contents.
    - The C compiler then compiles the source code. This involves translating the source code into assembly language.
    - The flags `-E` and can be used to perform preprocessing only.
