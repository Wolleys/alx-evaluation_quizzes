## Evaluation #8
### Evaluation Quiz: Evaluation #8 - Answers

#### Q0. When you are typing `https://www.google.com` in your browser, which HTTP verb is used?
- [x] GET
- [ ] PUT
- [ ] POST
- [ ] DELETE
- [ ] CREATE
- [ ] I don't know

#### Q1. What is the name of the HTTP request header that defines the size (in bytes) of the message body?
- [x] Content-Length
- [ ] Length
- [ ] Content-Size
- [ ] Size
- [ ] I don't know

#### Q2. A firewall can monitor ____________ traffic.
- [x] Incoming
- [x] Outgoing
- [ ] SQL Injections
- [ ] CPU Usage
- [ ] I don't know

#### Q3. What is the correct combination of `oflags` used to open a file with the mode write only and create it if it doesn’t exist?
- [ ] `O_WRONLY`
- [ ] `O_WRONLY | O_CREAT | O_EXCL`
- [x] `O_WRONLY | O_CREAT`
- [ ] `O_RDWR | O_CREAT`
- [ ] I don't know

#### Q4. What is the OSI model?
- [ ] Set of specifications that network hardware manufacturers must respect
- [x] The OSI model is a conceptual model that characterizes the communication functions of a telecommunication system without regard to their underlying internal structure and technology
- [ ] The OSI model is a model that characterizes the communication functions of a telecommunication system with a strong regard for their underlying internal structure and technology
- [ ] I don't know

#### Q5. Given this code:
```C
struct point {
   int x;
   int y;
};
struct point my_point = { 3, 7 };
struct point *p = &my_point;
```
To set the member `y` of my variable `my_point` to `98`, I can do (select all valid answers):

- [x] `(*p).y = 98;`
- [x] `p->y = 98;`
- [x] `my_point.y = 98;`
- [ ] `my_point->y = 98;`
- [ ] `p.y = 98;`
- [ ] I don't know

#### Q6. Based on this code, what should all the test cases be?
```python
def uniq(list):
    """ Returns unique values of a list """
    u_list = []
    for item in list:
        if item not in u_list:
            u_list.append(item)
    return u_list
```
(select multiple)

- [x] empty list
- [x] list with one element (any type)
- [x] list with 2 different elements (same type)
- [x] list with the same element twice (same type)
- [x] list with more than 2 times the same element (same type)
- [x] list with multiple types (integer, string, etc...)
- [x] not a list argument (ex: passing a dictionary to the method)
- [ ] I don't know

#### Q7. What is `__repr__`?
- [ ] Instance method that prints an "official" string representation of an instance
- [x] Instance method that returns an "official" string representation of an instance
- [ ] Instance method that returns the dictionary representation of an instance
- [ ] I don't know


















