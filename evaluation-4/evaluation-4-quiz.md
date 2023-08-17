## Evaluation #4
### Evaluation Quiz: Evaluation #4 - Answers

#### Q0. What data structure is the foundation of a Python dictionary or set?
- [x] Hash Table
- [ ] Stack
- [ ] Queue
- [ ] Binary Tree
- [ ] I don't know

#### Q1. What is the size of the `int` data type on a 64-bit machine?
- [ ] 1 byte
- [ ] 2 bytes
- [x] 4 bytes
- [ ] 8 bytes
- [ ] I don't know

#### Q2. What is `__doc__`?
- [ ] The string documentation of an object (based on docstring)
- [x] Prints the documentation of an object
- [ ] Creates man file
- [ ] I don't know

#### Q3. What is `__repr__`?
- [ ] Instance method that prints an "official" string representation of an instance
- [x] Instance method that returns an "official" string representation of an instance
- [ ] Instance method that returns the dictionary representation of an instance
- [ ] I don't know

#### Q4. Bubble Sort is a _______________.
- [x] simple comparison sorting algorithm
- [ ] complex comparison sorting algorithm
- [ ] simple non-comparison searching algorithm
- [ ] simple non-comparison sorting algorithm
- [ ] I don't know

#### Q5. Which of the following sorting algorithms has best case time complexity of `O(nlog(n))`?
- [x] Quick Sort
- [ ] Bubble Sort
- [ ] Insertion Sort
- [ ] Selection Sort
- [ ] I don't know

#### Q6. Given this code:
```C
struct point {
   int x;
   int y;
};
struct point my_point = { 3, 7 };
struct point *p = &my_point;
```
To set the member y of my variable `my_point` to 98, I can do (select all valid answers):

- [x] `my_point.y = 98`
- [x] `my_point->y = 98`
- [ ] `p.y = 98`
- [ ] `(*p).y = 98`
- [ ] `p->y = 98`
- [ ] I don't know

#### Q7. Based on this code, what should all the test cases be?
(select all possible answers)
```python
def uniq(list):
    """ Returns unique values of a list """
    u_list = []
    for item in list:
        if item not in u_list:
            u_list.append(item)
    return u_list
```
- [ ] empty list
- [x] list with one element (any type)
- [ ] list with 2 different elements (same type)
- [ ] list with the same element twice (same type)
- [x] list with more than 2 times the same element (same type)
- [x] list with multiple types (integer, string, etc...)
- [ ] not a list argument (ex: passing a dictionary to the method)
- [ ] I don't know

#### Q8. What is the `unistd` symbolic constant for the standard error?
- [ ] STDIN_FILENO
- [x] STDOUT_FILENO
- [ ] STDERR_FILENO
- [ ] I don't know

#### Q9. What do these lines print?
```python
>>> class User:
>>>     id = 89
>>>     name = "no name"
>>>     __password = None
>>>     
>>>     def __init__(self, new_name=None):
>>>         self.is_new = True
>>>         if new_name is not None:
>>>             self.name = new_name
>>> 
>>> u = User()
>>> u.name
```
- [ ] name
- [x] None
- [ ] 'John'
- [ ] 'no name'
- [ ] I don't know

#### Q10. What do these lines print?
```python
class Base():
    """ My base class """

    __nb_instances = 0

    def __init__(self):
        Base.__nb_instances += 1
        self.id = Base.__nb_instances

class User(Base):
    """ My User class """

    def __init__(self):
        super().__init__()
        self.id += 99

u = User()
print(u.id)
```
- [ ] 99
- [x] 100
- [ ] 1
- [ ] I don't know

#### Q11. In a singly linked list, what are possible directions to traverse it?
(select all possible answers)
- [x] Forward
- [ ] Backward
- [ ] I don't know

#### Q12. What do these lines print?
```python
class Base():
    """ My base class """

    __nb_instances = 0

    def __init__(self):
        Base.__nb_instances += 1
        self.id = Base.__nb_instances

class User(Base):
    """ My User class """

    def __init__(self):
        super().__init__()
        self.id = 89

u = User()
print(u.id)
```
- [ ] 89
- [x] 90
- [ ] 1
- [ ] I don't know

#### Q13. Is this module correctly documented?
```python
#!/usr/bin/python3
""" 
    My calculation module
"""
import sys
...
```
- [ ] Yes
- [x] No
- [ ] I don't know

#### Q14. Is this a standardized way to comment a function in Python?
```python
/* Addition function */
def add(a, b):
    return a + b
```
- [x] No
- [ ] Yes
- [ ] I don't know

#### Q15. What do these lines print?
```python
class User:
    id = 1

u = User()
User.id = 98
print(u.id)
```
- [ ] None
- [ ] 1
- [ ] 89
- [x] 98
- [ ] I don't know

#### 16. What does the following Bash script do?
```bash
#!/usr/bin/env bash                                                             

var="Tech"
if [ -e "$var" ]
then
    if [ -f "$var" ]
    then
        echo "Betty"
    elif [ -d "$var" ]
    then
        echo "School"
    fi
else
    echo "$var doesn't exist"
fi
```
- [x] Checks if `Tech` exists, otherwise prints "Tech doesn't exist". If it exists and it's a file, print "Betty", otherwise if it's a directory, print "School".
- [ ] Checks if a file (inputted by the user) exists, otherwise prints "File doesn't exist". If it exists and it's a file, print "Betty", otherwise if it's a directory, print "School".
- [ ] Checks if `Tech` exists and prints "Tech exists"
- [ ] I don't know

#### Q17. In this following code, what is`__password`?
```python
class User:
    id = 89
    name = "no name"
    __password = None

    def __init__(self, new_name=None):
        self.is_new = True
        if new_name is not None:
            self.name = new_name
```
- [ ] A public class attribute
- [ ] A public instance attribute
- [ ] A protected class attribute
- [x] A protected instance attribute
- [ ] A private class attribute
- [ ] A private instance attribute
- [ ] I don't know
