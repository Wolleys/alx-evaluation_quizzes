## Evaluation #5
### Evaluation Quiz: Evaluation #5 - Answers

#### Q0. What is the `/School/` regexp matching?
Select all valid answers
- [ ] scho0l
- [x] School
- [ ] school
- [ ] I don't know

#### Q1. What does the macro `TABLESIZE` expand to?
```console
#define BUFSIZE 1220
#define TABLESIZE BUFSIZE
#undef BUFSIZE
#define BUFSIZE 49
```
- [ ] 1220
- [x] 49
- [ ] nothing
- [ ] I don't know

#### Q2. What is the time complexity of removing at index `n` in an unsorted array?
- [ ] O(1)
- [x] O(n)
- [ ] O(n!)
- [ ] O(n^2)
- [ ] O(log(n))
- [ ] O(nlog(n))
- [ ] O(2^n)
- [ ] I don't know

#### Q3. The Internet Control Message Protocol (ICMP) is a protocol in the Internet protocol suite. It is used by network devices, to check if other network devices are available on the network. Which command uses ICMP to make sure that a network device remains online or to troubleshoot issues on the network?
- [x] `ping`
- [ ] `nc`
- [ ] `telnet`
- [ ] `grep`
- [ ] I don't know

#### Q4. What is the time complexity of this function / algorithm?
```python
void f(unsigned int n)
{
    int i;

    for (i = 1; i < n; i = i * 2)
    {
        printf("[%d]\n", i);
    }
}
```
- [ ] O(1)
- [x] O(n)
- [ ] O(n!)
- [ ] O(n^2)
- [ ] O(log(n))
- [ ] O(nlog(n))
- [ ] O(2^n)
- [ ] I don't know

#### Q5. Is this a standardized way to comment a function in Python?
```python
// Addition function
def add(a, b):
    return a + b
```
- [x] No
- [ ] Yes
- [ ] I don't know

#### Q6. What is the OSI model?
- [ ] Set of specifications that network hardware manufacturers must respect
- [x] The OSI model is a conceptual model that characterizes the communication functions of a telecommunication system without regard to their underlying internal structure and technology
- [ ] The OSI model is a model that characterizes the communication functions of a telecommunication system with a strong regard for their underlying internal structure and technology
- [ ] I don't know

#### Q7. What is `localhost`?
- [x] A hostname that refers to the current computer used to access it
- [ ] An IP address for the current computer used to access it
- [ ] A hostname that refers to all computers
- [ ] An IP address meaning "all IPv4 addresses"
- [ ] I don't know

#### Q8. What is `0b001010010` in base10?
- [ ] 81
- [ ] 82
- [ ] 83
- [x] 84
- [ ] I don't know

#### Q9. What are the layers of the OSI model?
- [x] Physical, Data Link, Network, Transport, Session, Presentation, Application
- [ ] Physical, Network, Transport, Presentation, Application
- [ ] Application, Session, Information, Packets, TCP/UDP
- [ ] Physical, Network, Transport, Session, Presentation, Application
- [ ] I don't know

#### Q10. What do these lines print?
```python
>>> def my_function(counter=89):
>>>     print("Counter: {}".format(counter))
>>> 
>>> my_function(12)
```
- [x] Counter: 12
- [ ] Counter: 89
- [ ] Counter: 101
- [ ] I don't know

#### Q11. What is the `/Scho.l/` regexp matching?
Select all valid answers
- [x] Scho.l
- [ ] School
- [ ] school
- [ ] I don't know

#### Q12. What command displays information about active processes?
- [x] `ps`
- [ ] `pgrep`
- [ ] `pkill`
- [ ] `kill`
- [ ] `trap`
- [ ] I don't know

#### Q13. What is the `/Scho*l/` regexp matching?
Select all valid answers
- [x] School
- [ ] Schol
- [ ] Scho.l
- [ ] Schooool
- [ ] I don't know

#### Q14. What command would you use to list files on Linux?
- [x] ls
- [ ] which
- [ ] cd
- [ ] pwd
- [ ] list
- [ ] I don't know

#### Q15. What is the time complexity of this function / algorithm?
```C
void f(int n)
{
    int i;
    int j;

    for (i = 0; i < n; i++)
    {
        if (i % 2 == 0)
        {
            for (j = 1; j < n; j = j * 2)
            {
                printf("[%d] [%d]\n", i, j);
            }
        }
        else
        {
            for (j = 0; j < n; j = j + 2)
            {
                printf("[%d] [%d]\n", i, j);
            }
        }
    }
}
```
- [ ] O(1)
- [x] O(n)
- [ ] O(n!)
- [ ] O(n^2)
- [ ] O(log(n))
- [ ] O(nlog(n))
- [ ] O(2^n)
- [ ] I don't know

#### Q16. What is `/etc/hosts`?
- [ ] A plain text file used to translate hostnames into IP addresses
- [ ] A Python script used to translate hostnames into IP addresses
- [x] A plain text file used to translate IP addresses into hostnames
- [ ] A plain text file used by other computers to know the name of your computer
- [ ] I don't know

#### Q17. What is a Makefile?
- [x] file which defines a set of tasks to be executed
- [ ] a command which makes a file to define a set of tasks to be executed
- [ ] a file that makes a new shell window
- [ ] I don't know

#### Q18. What command would you use to stop a process named `dontstopmenow`?
- [ ] `pkill -f dontstopmenow`
- [ ] `kill -f dontstopmenow`
- [x] `kill dontstopmenow`
- [ ] `pgrep -f dontstopmenow`
- [ ] I don't know
