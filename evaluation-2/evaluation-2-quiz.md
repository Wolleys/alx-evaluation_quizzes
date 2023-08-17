## Evaluation #2
### Evaluation Quiz: Evaluation #2 - Answers

#### Q0. Without context, on Ubuntu 14.04 LTS, `write` is a(n) …
(please select all correct answers)
- [ ] executable
- [x] system call
- [ ] library call
- [ ] game
- [ ] I don't know

#### Q1. What is0b001010010 in base10?
- [ ] 81
- [x] 82
- [ ] 83
- [ ] 84
- [ ] I don't know

#### Q2. When I am using `O_WRONLY | O_CREAT | O_APPEND` -> the `|` are bitwise operators.
- [x] True
- [ ] False
- [ ] I don't know

#### Q3. What is the `unistd` symbolic constant for the standard input?
- [x] STDIN_FILENO
- [ ] STDOUT_FILENO
- [ ] STDERR_FILENO
- [ ] I don't know

#### Q4. What are the different steps to form an executable file from C source code?
- [ ] Interpretation, compilation and assembly
- [x] Preprocessing, compilation, assembly, and linking
- [ ] Interpretation, assembly and compilation
- [ ] Compilation and linking
- [ ] Preprocessing and compilation
- [ ] I don't know

#### Q5. Choose the line of code to replace the comment below so the function prints a given string without a lower or uppercase `c`.
```bash
>>>def no_c_print(s):
...    new_string = ''
...    for character in s:
...        # REPLACE THIS LINE              
...           new_string += character
...    print(new_string)
...
>>> no_c_print("Characters")
>>>haraters
```
- [ ] `if character not in 'Cc':`
- [x] `if character != 'c' and character != 'C':`
- [ ] `if character != "cC"`
- [ ] I don't know

#### Q6. The following code gives this incorrect output.
Which of the following statements about what is causing the error is true? (select all valid answers)

```bash
carrie@ubuntu:/debugging$ cat main.c                               
#include <stdio.h>                                                                                 

/**                                                                                                
 * main - debugging example                                                                        
 * Return: 0                                                                                       
 */                                                                                                
int main(void)                                                                                     
{                                                                                                  
        int i;                                                                                     
        int j;                                                                                     

        for (i = 0; i < 10; i++)                                                                   
        {                                                                                          
                j = 0;                                                                             
                while (j < 10)                                                                     
                {                                                                                  
                        printf("%d", j);                                                           
                }                                                                                  
                printf("\n");                                                                      
        }                                                                                          

        return (0);                                                                                
}                                                                                                  
carrie@ubuntu:/debugging$
```

```bash
carrie@ubuntu:/debugging$ gcc -Wall -Werror -Wextra -pedantic main.c                                                                                                  
carrie@ubuntu:/debugging$ ./a.out
0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 <...>
^Ccarrie@ubuntu:/debugging$
```
- [x] `j` never increments so it will always be less than `10`
- [ ] `j` is always equal to `i` so the loop will never end
- [ ] `j` never increments so it is always going to print `0`
- [ ] I don't know















