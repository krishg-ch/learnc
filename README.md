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
1. A C compiler --> 
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
}
```
