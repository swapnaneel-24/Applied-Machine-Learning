1. print--> print something on display screen --- but loggs ... document --> logs
2. input --> to take the input from the user


```python
print("Anything you can ask me ")
```

    Anything you can ask me 
    


```python
input()
```

     hello
    




    'hello'




```python
print('Enter something as input: ')
input()
```

    Enter something as input: 
    

     2345678
    




    '2345678'




```python
input("Enter something as input: ")
```

    Enter something as input:  46578
    




    '46578'



to store store something  varaible address


```python
 a = input('ENter something : ')
```

    ENter something :  123
    


```python
101101001001 = 123
```


      Cell In[9], line 1
        101101001001 = 123
        ^
    SyntaxError: cannot assign to literal here. Maybe you meant '==' instead of '='?
    


never start number , *&^$%#@!

combination of alphabet, numbers , _
conditions related to 
1. ist character must not be number
2. the numbers have to come along with alphabet or _

q1 valid, 2  not valid, 3ert not valid, 4567 not valid, _4 valid


```python
_4 = "qwert"
```


```python
_ = 34
print(_)
```

    34
    

#  Date type
1. Number type
    a) int
    b) float
    c) complex
2. Text type
   a) string
3. List
4. tuple
5. set
6. dictionary
7. array --> Numpy

# Array 
1. array size is fix
2. homogeneous data type--- array store only 1 type of data
3. we can access any data directly using the indexing
4. continuous memory

array size is 40 
int a= [23,45, 67, 89,'rt']

a---> 41,42

42
a -->[23,45, 67, 89, 41,42]

string:'', ""

a = 'Hello'
     01234  

iterator--> the data type on which you can do the indexing

for loop
1. using Range Function
2. using iterator

#### using iterator


```python
A = "HELLO"
for i in A:
    print(i)
```

    H
    E
    L
    L
    O
    


```python
a = 4567 #- int
for i in a:
    print(i)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[16], line 2
          1 a = 4567
    ----> 2 for i in a:
          3     print(i)
    

    TypeError: 'int' object is not iterable



```python
a = '4567'
for i in a:
    print(i)
```

    4
    5
    6
    7
    


```python
listo = [23,56,78,94,34]
```


```python

for i in listo:
    print(i)
```

    23
    56
    78
    94
    34
    


```python
tup = (23,56,78,90,34)
for i in tup:
    print(i)
```

    23
    56
    78
    90
    34
    

### using Range Function

range(start, stop, step)

### constraints
1. range(with single value) --> start = 0 (by default), stop< that single value , step = 1 (by default)
2. range(with 2 values) --> start = the first value u have passed , stop < 2nd value , step = 1 (by default)
3. range(with 3 values) --> start = first value, stop < second value , step = 3rd value


```python
for i in range(4):
    print(i)
```

    0
    1
    2
    3
    


```python
for i in range(2, 4):
    print(i)
```

    2
    3
    


```python
for i in range(2, 8,2):
    print(i)
```

    2
    4
    6
    


```python
listo = [23,56.89,'rafa', [23,65], (3,4),{'a':23}]

```


```python
for val in listo:
    print(val)
    print(".....")
```

    23
    .....
    56.89
    .....
    rafa
    .....
    [23, 65]
    .....
    (3, 4)
    .....
    {'a': 23}
    .....
    


```python
listo = [23,56.89,'rafa', [23,65], (3,4),{'a':23}]
print(len(listo))
for val in range(len(listo)):  # range always takes integer number
    print(listo[val])
```

    6
    23
    56.89
    rafa
    [23, 65]
    (3, 4)
    {'a': 23}
    


```python
for val in range(6):
    print(val)
```

    0
    1
    2
    3
    4
    5
    


```python
def calcu():
    a = int(input('Enter ist: '))
    b = int(input('Enter 2nd: '))
    return a+b
    
    
```


```python
def calcu():
    a = int(input('Enter ist: '))
    b = int(input('Enter 2nd: '))
    return a+b
    print('Hello')
    
```

## return
1. it terminates the function
2. it returns to the position from where you are calling it


```python
acb = calcu()
```

    Enter ist:  45
    Enter 2nd:  67
    


```python
print(acb)
```

    112
    


```python
calcu()
```

    Enter ist:  6789
    Enter 2nd:  876543
    




    883332



### Parameter and argument



```python
a = 34
c = a+b
```


```python
def hy(b,a=45):
    print(a)
    print(b)
    print(a+b)

```


```python
hy(b=3, a = 6777)
```

    6777
    3
    6780
    


```python
def hy(b,a=45):
    print(a)
    print(b)
    print(a+b)
    print('Hello Kya hal chal')
```


```python
hy(2,5)
```

    5
    2
    7
    Hello Kya hal chal
    


```python
def hy(b,a=45):
    print(a)
    print(b)
    print(a+b)
    return
    print('Hello Kya hal chal')
```


```python
hy(45,89)
```

    89
    45
    134
    

## Recursions

1. base condition
2. termination condition
3. function calling



```python
for i in range(0, 20, 5):
    print(i)
# base condition = 0
# termination condition <20
```

    0
    5
    10
    15
    


```python
def reccc(i):
    if i ==20:
        return
    print(i)
    reccc(i+5)

 #i=0, 5 ,10  
```


```python
reccc(0)
```

    0
    5
    10
    15
    


```python
# find the sum of first 5 numbers, 0,1,2,3,4

sumz =0 
for i in range(5):
    sumz += i
print(sumz)
```

    10
    


```python
def sumz(i):
    if i==5:
        return 0
    return i + sumz(i+1)

```


```python
sumz(0)
```




    10




```python

```
