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
```C
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

```C
user@ubuntu:/debugging$ cat main.c                               
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
user@ubuntu:/debugging$
```

```bash
user@ubuntu:/debugging$ gcc -Wall -Werror -Wextra -pedantic main.c                                                                                                  
user@ubuntu:/debugging$ ./a.out
0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 <...>
^Cuser@ubuntu:/debugging$
```
- [x] `j` never increments so it will always be less than `10`
- [ ] `j` is always equal to `i` so the loop will never end
- [ ] `j` never increments so it is always going to print `0`
- [ ] I don't know

#### Q7. Choose a statement that would complete the function that returns a string made up of `+` `n` number of times (assuming `n` > 0).
```C
>>> def print_plus(n):
...         # REPLACE THIS LINE
...
>>> print_plus(3)
>>> '+++'
>>> print_plus(4)
>>> '++++'
```
- [ ] `return n*'+'`
- [x] `return '+'*n`
- [ ] `return ''+n`
- [ ] `return+n+n+n`
- [ ] I don't know

#### Q8. In the main.c file, on what line is the first error that the compiler returns?
Look at the following code.

```C
user@ubuntu:/debugging$ cat main.c                                
#include <stdio.h>                                                                                  

/**                                                                                                 
 * main - debugging example                                                                         
 * Return: 0                                                                                        
 */                                                                                                 
int main(void)                                                                                      
{                                                                                                   
        char *hello = "Hello, World!";                                                              

        for (i = 0; hello[i] != '\0'; i++)                                                          
        {                                                                                           
                printf("%c", hello[i]);                                                             
        }                                                                                           

        printf("\n");                                                                               

        return (0);                                                                                 
}                                                                                                   
user@ubuntu:/debugging$
```

```bash
user@ubuntu:/debugging$ gcc -Wall -Werror -Wextra -pedantic main.
c                                                                                                   
main.c: In function ‘main’:                                                                         
main.c:11:7: error: ‘i’ undeclared (first use in this function)                                     
  for (i = 0; hello[i] != '\0'; i++)                                                                
       ^                                                                                            
main.c:11:7: note: each undeclared identifier is reported only once for each function it appears in
main.c:9:8: error: variable ‘hello’ set but not used [-Werror=unused-but-set-variable]              
  char *hello = "Hello, World!";                                                                    
        ^                                                                                           
cc1: all warnings being treated as errors                                                           
user@ubuntu:/debugging$ 
```
- [ ] 9
- [x] 11
- [ ] 7
- [ ] I don't know

#### Q9. What is `98` in base 16?
- [x] `0x62`
- [ ] `0x98`
- [ ] `0x96`
- [ ] I don't know

#### Q10. What does this command line print?
```C
>>> a = "Hello, world!"
>>> print(a[:5])
```
- [ ] Hello
- [x] world!
- [ ] orld!
- [ ] I don't know

#### Q11. `0x13 << 1` = ?
- [x] 0x13
- [ ] 0x12
- [ ] 0x26
- [ ] 0x4C
- [ ] I don't know

#### Q12. What is the correct combination of `oflags` used to open a file with the mode write only, create it if it doesn’t exist and append new content at the end if it already exists?
- [ ] `O_WRONLY`
- [ ] `O_WRONLY | O_CREAT | O_EXCL`
- [x] `O_WRONLY | O_CREAT | O_APPEND`
- [ ] `O_RDWR | O_CREAT | O_APPEND`
- [ ] I don't know

#### Q13. What is wrong with the following code?
```C
int n = 0;
int array[5];
int i = 5;

array[n] = i;
```
- [ ] Nothing is wrong
- [ ] It is impossible to declare the variable `array` this way
- [x] The array `array` is not entirely initialized
- [ ] It is not possible to access `array[n]`
- [ ] I don't know

#### Q14. What does this print?
```C
>>> print("My favorite line of {} is {:d}.".format("The Zen of Python", 11))
```
- [ ] My favorite line of The Zen of Python is 11.
- [ ] My favorite line of T is 1.
- [ ] My favorite line of The Zen of Python is 1.
- [x] I don't know

#### Q15. `~ 0x98 =` ?
- [ ] `0x66`
- [ ] `0x67`
- [x] `0x68`
- [ ] I don't know
