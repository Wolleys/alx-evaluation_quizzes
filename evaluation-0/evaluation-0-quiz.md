## Evaluation #0
### Evaluation Quiz: Evaluation #0 - Answers

#### Q0. What command would you use to list files on Linux?
- [x] ls
- [ ] which
- [ ] cd
- [ ] pwd
- [ ] list
- [ ] I don't know

#### Q1. What are the different steps to form an executable file from C source code?
- [ ] Interpretation, compilation and assembly
- [x] Preprocessing, compilation, assembly, and linking
- [ ] Interpretation, assembly and compilation
- [ ] Compilation and linking
- [ ] Preprocessing and compilation
- [ ] I don't know 

#### Q2. What is the problem with the following C code?
```C
#include <stdio.h>

/**
* main - main function 
* Return: 0
*/

int main(void)
{
        int i;

        i = 65;

        while (i < 91)
        {
                putchar(i);
        }

        return (0);
}
```

- [ ] `i` is not incremented in the while loop, so an infinite loop occurs
- [x] `i` is not incremented outside the loop, so an infinite loop occurs
- [ ] You cannot use integers in `putchar()`
- [ ] I don't know

#### Q3. What is the size of the `float` data type on a 64-bit machine?
- [ ] 1 byte
- [ ] 2 bytes
- [ ] 4 bytes
- [x] 8 bytes
- [ ] I don't know

#### Q4. What is the numerical value for the `r-xr--r--` permission?
- [ ] 522
- [ ] 544
- [ ] 644
- [x] 411
- [ ] I don't know

#### Q5. What does this code print?
```C
* print_something - function to print something
*
* Return: Always 0
**/
int print_something(int num)
{
    int i, j;
    for (i = 0; i < num + 1; i++)
    {
        for (j = 0; j < num + 1; j++)
        {
            printf("%d", i * j);
            if (j < num)
            {
                printf(", ");
            }
        }
        printf("\n");
    }
    return (0);
}
```

- [ ] The `n` times table, starting with 0
- [ ] The `n` times table, excluding zero
- [x] The numbers 0 to `n`, `n` times
- [ ] I don't know

#### Q6. What information do the `printf` statements tell us about how our code is executed?
This code doesn’t work as intended.
```C
#include "school.h"

/**
* main - prints even numbers from 0 to 100
* Return: 0
*/

int main(void)
{
        int i;

        for (i = 0; i < 100; i++)
        {
                if (i % 2 != 0)
                {
                        continue;
                }
                else
                {
                        break;
                }

                printf("%d\n", i);
        }

        return(0);
}
```
Let’s add `printf` statements to the code.

```C
#include "school.h"

/**
* main - prints even numbers from 0 to 100
* Return: 0
*/

int main(void)
{
        int i;

        printf("Before loop\n");

        for (i = 0; i < 100; i++)
        {
                if (i % 2 != 0)
                {
                        printf("i is not even so don't print\n");
                        continue;
                }
                else
                {
                        printf("i is even, break to print\n");
                        break;
                }

                printf("Outside of if/else, still inside for loop\n");

                printf("%d\n", i);
        }

        printf("For loop exited\n");

        return(0);
}
```
What information do the `printf` statements tell us about how our code is executed? (select all valid statements)

- [ ] A `printf` statement shows when the for loop is finished
- [x] A `printf` statement shows exactly how many times the loop executes
- [x] `printf` statements shows that break will cause "For loop exited" to print, indicating that the even number is never printed
- [ ] A `printf` statement shows that there is an infinite loop in the code
- [ ] I don't know

#### Q7. What shape will this code print?
```C
#include <stdio.h>

/**
* print_shape - function to print a shape
*/
void print_shape(int num1, int num2) 
{
    int idx1, idx2;
    for (idx1 = 0; idx1 < num1; idx1++)
    {
        for (idx2 = 0; idx2 < num2; idx2++)
        {
            printf('#');
        }
        printf('\n');
    }
}

/** 
* main - calls print_shape()
*
* Return: Always 0.
**/

int main(void)
{
    print_shape(4, 3);
    return (0);
}
```
- [x] A rectangle with the character `#` with a height of 4 and width of 3
- [ ] A rectangle with the character `#` with a height of 3 and width of 4
- [ ] A triangle with the character `#` with a base of 4 and height of 3
- [ ] A rectangle with the character `*` with a height of 4 and width of 3
- [ ] I don't know

#### Q8. Which command should I use for changing a file owner?
- [ ] `su`
- [ ] `chmod`
- [x] `chown`
- [ ] `chgrp`
- [ ] I don't know

#### Q9. Which of these loop statements exist in C?
Select all valid answers
- [x] for
- [x] while
- [ ] foreach
- [x] do...while
- [ ] loop_to
- [ ] each
- [ ] I don't know

#### Q10. Which command should I use to display the exit code of the previous command?
- [ ] `echo ?`
- [ ] `echo $EXITCODE`
- [ ] `echo $CODE`
- [x] `echo $?`
- [ ] I don't know

#### Q11. What is the output of the following piece of code?
```C
int i;

i = 10;
while (i < 20)
{
    printf("%d", i % 2);
    i++;
}
```

- [x] 0101010101
- [ ] 0123456789
- [ ] 1010101010
- [ ] I don't know 

#### Q12. How do you change directory on Linux?
- [ ] pwd
- [x] cd
- [ ] ls
- [ ] which
- [ ] I don't know

#### Q13. Which symbol should I use to redirect the error output to the standard output?
- [x] 2>&1
- [ ] 1>&2
- [ ] 2>
- [ ] I don't know
