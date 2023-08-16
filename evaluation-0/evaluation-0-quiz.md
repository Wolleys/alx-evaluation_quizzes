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
