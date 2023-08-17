## Evaluation #6
### Evaluation Quiz: Evaluation #6 - Answers

#### Q0. If we were to print the following tree using pre-order traversal, what would you expect the output to be?
```console
.-------(098)-------.
  .--(012)--.         .--(402)-------.
(010)     (054)     (045)       .--(128)--.
                              (092)     (065)
```
- [ ] 98, 12, 10, 54, 402, 45, 128 ,92, 65
- [ ] 98, 12, 402, 10, 54, 45, 128, 92, 65
- [x] 10, 12, 54, 98, 45, 402, 92, 128, 65
- [ ] 10, 54, 12, 45, 92, 65, 128, 402, 98
- [ ] I don't know

#### Q1. What is TCP/IP?
- [ ] Transmission Control Protocol/Internet Protocol, is a suite of communications protocols used to interconnect network devices on the Internet or any private network.
- [x] Transmission Control Protocol/Internet Protocol, is a suite of communications protocols used to interconnect network devices on the Internet.
- [ ] Transmission Control Protocol/Internet Protocol, is a suite of communications protocols used to interconnect network devices on private network.
- [ ] I don't know

#### Q2. A firewall can monitor ________________ traffic.
Please select all valid answers.
- [x] Incoming
- [x] Outgoing
- [ ] SQL Injections
- [ ] CPU Usage
- [ ] I don't know

#### Q3. What do these lines print?
```python
>>> a = { 'id': 89, 'name': "John", 'projects': [1, 2, 3, 4], 'friends': [ { 'id': 82, 'name': "Bob" }, { 'id': 83, 'name': "Amy" } ] }
>>> a.get('friends')[-1].get("name")
```
- [ ] 89
- [ ] [{'id':82, 'name':"Bob"}, {'id':83, 'name': "Amy"}]
- [x] 'Amy'
- [ ] 'Bob'
- [ ] Nothing
- [ ] I don't know

#### Q4. What is the size of `*p` in this code?
`int **p;`
- [x] 4 bytes
- [ ] 8 bytes
- [ ] 16 bytes
- [ ] 32 bytes
- [ ] I don't know

#### Q5. Which command should I use to display the exit code of the previous command?
- [ ] `echo ?`
- [ ] `echo $EXITCODE`
- [ ] `echo $CODE`
- [x] `echo $?`
- [ ] I don't know

#### Q6. What is a database?
- [ ] a collection of text files that are stored so that it can be easily accessed, updated and managed by the local application
- [ ] a collection of information that is stored on a physical server and organized so that it can be easily accessed, updated and managed
- [x] a collection of information that is stored and organized so that it can be easily accessed, updated and managed
- [ ] I don't know

#### Q7. Given this code:
```C
struct point {
   int x;
   int y;
};
struct point my_point = { 3, 7 };
struct point *p = &my_point;
```
To set the member `y` of my variable `my_point` to `98`, I can do (select all valid answers):
- [ ] `my_point.y = 98;`
- [ ] `my_point->y = 98;`
- [x] `p.y = 98;`
- [ ] `(*p).y = 98;`
- [x] `p->y = 98;`
- [ ] I don't know

#### Q8. What is a server?
- [x] A server is a device, a virtual device or computer program or providing functionality for other programs or devices, called “clients”.
- [ ] A server is a software that serves web pages.
- [ ] A server is returning information to other computers when asked.
- [ ] I don't know

#### Q9. Based on this code, what should all the test cases be?
```python
def uniq(list):
    """ Returns unique values of a list """
    u_list = []
    for item in list:
        if item not in u_list:
            u_list.append(item)
    return u_list
```
Select all valid answers
- [ ] empty list
- [x] list with one element (any type)
- [ ] list with 2 different elements (same type)
- [ ] list with the same element twice (same type)
- [ ] list with more than 2 times the same element (same type)
- [x] list with multiple types (integer, string, etc...)
- [ ] not a list argument (ex: passing a dictionary to the method)
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
- [ ] 1
- [ ] 99
- [x] 100
- [ ] I don't know

#### Q11. You will not be able to reconnect to your server via SSH - and will not be able to recover it - if you ever deny port _____
- [ ] 80
- [x] 22
- [ ] 440
- [ ] 12
- [ ] I don't know

#### Q12. Which command grants or removes other users’ privileges in MySQL?
- [x] GRANT OPTION
- [ ] SUDO
- [ ] CHANGE OWNER
- [ ] SWITCH
- [ ] I don't know

#### Q13. In the context of web infrastrucutre, what is SPOF?
- [x] "Single Point of Failure" - A part of a system that will stop the entire system if it fails
- [ ] "Single Point of Failure" - A part of the system designed to fail if other parameters are met
- [ ] "Single Point of Freedom" - When your server is set up to only allow requests from a single specified IP address
- [ ] "Spare Parts Order Form" - A form used to request backup hardware
- [ ] I don't know

#### Q14. An object-relational mapper (ORM) . . .
Please select all valid answers
- [x] is a code library that automates the transfer of data stored in relational databases tables into objects
- [ ] provides a high-level abstraction upon a relational database
- [ ] allows a developer to write Python code instead of SQL
- [ ] I don't know

#### Q15. What line(s) would you replace `# REPLACE THIS LINE` with in the following code?
```python
#!/usr/bin/env python3
"""
Script that lists all State objects from a database
"""
if __name__ == "__main__":
    # Import necessary modules
    from sys import argv
    from sqlalchemy import create_engine
    from sqlalchemy.orm import sessionmaker
    from model_state import State

    # Set variables to input arguments
    username = argv[1]
    password = argv[2]
    db_name = argv[3]

    # Start engine
    engine = create_engine('mysql+mysqldb://{}:{}@localhost/{}'.format(username, password, db_name))

    # Create a configured class Session
    Session = sessionmaker(bind=engine)

    # Create a Session instance
    my_session = Session()

    # my_session work
    # REPLACE THIS LINE
    for object in objects: 
        print("{}: {}".format(object.id, object.name))

    # Close session
    my_session.close()
```
- [ ] objects = my_session.query(State).order_by(State.id).all()
- [x] my_session.execute("SELECT states.id, states.name FROM states ORDER BY id ASC") objects = my_session.fetchall()
- [ ] objects = my_session.find(State).order_by(State.id).all()
- [ ] I don't know

#### Q16. Which MySQL command enables a user to delete tables or databases?
- [x] DROP
- [ ] DELETE
- [ ] REMOVE
- [ ] KILL
- [ ] I don't know

#### Q17. Which of the following statements about what is causing the error is true? (select all valid answers)
The following code gives this incorrect output
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

user@ubuntu:/debugging$ gcc -Wall -Werror -Wextra -pedantic main.c                                                                                                  
user@ubuntu:/debugging$ ./a.out
0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 <...>
^Ccarrie@ubuntu:/debugging$
```
Which of the following statements about what is causing the error is true?
- [x] `j` is always equal to `i` so the loop will never end
- [x] `j` never increments so it will always be less than `10`
- [x] `j` never increments so it is always going to print `0`
- [ ] I don't know

#### Q18. What is in-order traversal?
- [x] the left subtree is visited first, then the root and later the right sub-tree
- [ ] the root node is visited first, then the left subtree and finally the right subtree
- [ ] left subtree is visited first, then the right subtree and finally the root node
- [ ] I don't know

#### Q19. In this following code, what is `__password`?
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
- [ ] A private class attribute
- [ ] A private instance attribute
- [ ] A protected instance attribute
- [ ] A protected class attribute
- [x] A public instance attribute
- [ ] A public class attribute
- [ ] I don't know
