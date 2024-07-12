# Learn C

> [!NOTE]
> <details>
> <summary>Expand to know about types of programming languages</summary>
> 
> ## Types of Programming Languages:
> ### 1. Low-Level Languages:
>    - Include machine language (binary) and assembly language.
>    - Provide direct access to computer`s hardware.
>    - Instructions closely correspond to specific machine instructions.
>    - They offer speed, efficiency, low memory consumption, and fine-grained control over hardware.
>    - **Machine language**:
>      - Consists of series of 0s and 1s that correspond directly to machine instructions.
>      - Instructions are executed directly by the processor.
>      - Not human-readable and time-consuming to write.
>    - **Assembly language**:
>      - Uses mnemonics and symbols corresponding to the machine's instruction set.
>      - Allows working closely with the machine on a slightly higher level.
> ### 2. High-Level Languages:
>    - Examples include Python and JavaScript.
>    - Far removed from a particular machine's instruction set.
>    - Syntax resembles the English language, making them easier to work with and understand.
>    - Programs are portable and machine-independent.
>    - Tend to be slower, consume more memory, and make it harder to work with low-level hardware.
> ### 3. Middle-Level Languages:
>    - Examples include C and C++.
>    - Act as a bridge between low-level and high-level languages.
>    - Allow for control over computer hardware while offering a level of abstraction.
>    - Instructions are more human-readable and understandable for programmers.
> </details>



## Background of C :
C was developed by Dennis M. Ritche and Brian W. Kernighan.
The origin of C is closely tied to the development of the Unix OS.
UNIX was initially written in the B language, C is introduced to overcome its shortcomings.
The C language was brought into the market in 1972, but became popular in 1978.

### Features :
* Flexible language, well-structured and organised code.
* Designed to provide low-level access to memory, thus requiring minimal run time support.
* Can be executed in different platforms with minimal changes.
* Support cross-platform programming, and can be compiled for a wide variety of computer platforms and operating systems.
* Available on a wide range of platforms, from embedded microcontrollers to supercomputers.

## Setup a Development Envrionment 

To write C programs in your local machine, you need:
1. A C compiler --> GCC via Mingw-w64 or C/C++ Extension in Visual Studio Code
2. An IDE --> [Visual Studio Code](https://code.visualstudio.com/)

## Structure of C program :

https://github.com/krishg-ch/learnc/blob/070434677682e6ac47fb6bd059743dee91aeeba5/src/sample.c?plain=1#L1-L21
```C
 /* Documentation section 
    (About the code) */ 
  
 #include<stdio.h>        // Link section 
  
 #define PI 3.14          // Definition section 
  
 void add();              // Global declaration section 
 int a = 2; 
  
 int main()               // Main function 
 { 
   // Body of the function 
   printf('This is a sample program'); 
   return 0;              // return value from main function 
 } 
  
 void add()               // Subprogram section 
 { 
   // Body of the subprogram 
 } 
```

### Header files in C:
1. Header files are external libraries, by adding them we get additional functionalities that we can use in the code.
2. #include is a preprocessor command that tells the C compiler to include a file.
3. stdio.h stands for standard input output, which contains function definitions for input and output operations. Eg: printf(), scanf() etc.

### Main function in C :
1. Every C program may have more than one fuction, which must include a main() function. It is the first thing that is called when the program is executed.
2. The int keyword in int main() {} indicates the return value of the main() function. So here it returns an integer number.
3. When calling a function, arguments are passed in between parentheses (), and if the main function has no parameters, the keyword "void" is used.
4. Anything inside the curly braces, {}, is considered the body of the function – here is where you include the code you want to write.

### Comments in C :
1. Comments are lines of text that get ignored by the compiler. Comments provide a way to document your code
2. There are two types of commenting styles :
   - Single line comments --> Anything after // in that line
   - Multi line comments --> Anything in between /* and */

### printf() in C :
1. printf() function is used when we want to display something.
2. Text to be displayed is placed in between " " inside the paranthesis ().
3. Every statement in C ends with semicolon (;). Think of this as a fullstop (.) in sentences.

### escape sequences in C :
1. An escape sequence is a combination of characters that represents a special character within a string.
2. They consist of a backslash, \, also known as the escape character, followed by one or more additional characters.
3. The escape sequence for a newline character is \n.

### Compile and run your C program :
The compilation of a C program consists of four steps: 
1. **Preprocessing phase** :
   - The preprocessor scans through the source code to find preprocessor directives, which are any lines that start with a # symbol, such as #include .
   - Once the preprocessor finds these lines, it substitutes them all the code from the header file.
2. **Compilation phase** :
   - This is where the modified source code gets translated into the corresponding assembly code.
   - If there are any errors, compilation will fail, and you will need to fix the errors to continue.
3. **Assembly phase** :
   - This is where the assembler converts the generated assembly code statements into machine code instructions.
   - The output of this phase is an object file, which contains the machine code instructions.
4. **Linking phase** :
   - Linking is the process of combining the object file generated from the assembly phase with any necessary libraries to create the final executable binary file.

![img\compilationprocess](https://github.com/krishg-ch/learnc/assets/87570647/26b4f456-d3e6-43c2-8229-f82920debbb0)

**To run the program** :
* Inside the terminal, type this for compiling :
  - gcc main.c
* Compiler output gives 'a.out' file in the directory.
* To run the file, type this :
  - ./a.out   (./ represents the current directory and a.out is the file name)
* To change the default exectubale name from a.out to different name, use this :
  - gcc -o <executablename> <filename>.c
 
## Variables and Datatypes
