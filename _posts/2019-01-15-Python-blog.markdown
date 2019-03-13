---
layout: post
title: Python Programming
date: 2019-01-15
Tags: Python
---
# Python Introduction

Python is a high-level, general-purpose programming language. Python is used for developing complex scientific and numeric applications. Python is one of the most popular languages for data analysis and visualization.

##  Variable



```python
a = 5            # Number is assigned to the variable
print(a)         # Output is 5

name = 'John'    #Number is assigned to the variable
print(name)    #Output is John
```

## Numbers

The numerics in python includes integer and float. 


```python
x = 1            # Integer is assigned
y = 2.8          # Floating number is assigned
```

## Strings


```python
print ('Hello! World!')       # prints Hello! World!
print ('Hello! \nWorld!')     # prints Hello! and World! in different line
print ('Hello!\tWorld!')      # prints Hello!  World! where there is spaces between Hello! and World!

word_length = len('Hello')    # gives the length of the words which is 5
```

### String: Indexing and Slicing

Indexing chooses selected index of strings and slicing grabs subsection of the string.


```python
word = 'Hello! World!'

print(word[0])     # prints H. Index always starts from 0 
print(word[8])     # prints o. Space between two words is also counted in indexing.
print(word[-3])    # prints l

print(word[2:])    # prints llo! World!
print(word[:3])    # prints Hel
print(word[2:5])   # prints llo
print(word[::2])   # prints Hlo ol!
print(word[2:11:2])# prints lo ol
print(word[::-1])  # prints !dlroW !olleH
```

###  String: Properties and Method


```python
word = 'Hello! World!'
word_add = word + 'Good morning'
word_multiple = word * 2

print(word_add)                   # Adds strings and prints Hello! World!Good morning
print(word_multiple)              # Multiplies word and prints two times i.e. Hello! World!Hello! World!
```


```python
word_upper = word.upper()    # changes all the letters to uppercase i.e. HELLO! WORLD!
word_lower = word.lower()    # changes all the letters to lowercase i.e. hello! world!
word_split = word.split()    # changes all the letters to split i.e. ['Hello!', 'World!']
```

### String: Print formatting 


```python
result = 100/6
word = 'Hello! World!'

print('{} Good morning'.format(word)) # prints Hello! World! Good morning
# prints Sam is smart and hardworking guy
print('Sam is {} and {} {}'.format('smart', 'hardworking', 'guy')) 
# prints Sam is smart and hardworking guy                                 
print('Sam is {2} {1} and {0} {1}'.format('hardworking', 'guy','smart')) 
# prints Sam is smart and hardworking guy                                  
print('Sam is {s} and {h} {g}'.format(h = 'hardworking', g = 'guy',s = 'smart')) 
# prints His name is John. John is the best guy.                              
print("His name is {0}. {0} is the best guy.".format('John'))
# prints result 16.666666666666668                                    
print('The result was {}'.format(result)) 
# prints result upto three decimal places i.e. 16.667                                  
print('The result was {r:1.3f}'.format(r = result))                                    
```

## Operators

Operators are used to perform operations on variables and values.

Python divides the operators in the following groups:

- Arithmetic operators
- Assignment operators
- Comparison operators
- Logical operators
 

### Operators: Arithmetic 

It includes addition, substraction, multiplication, division, modulus and power


```python
a = 5       #Assigns value
b = 2       #Assigns value
c = a + b   #Addtion to give 7
d = a - b   #Subtraction to give 3
e = a * b   #Multiplication to give 10
f = a / b   #Division to give 2.5
g = a % b   #Mduli to give 1
h = a ** b  #Power to give 25

```

### Operators: Assignment 

It is used to assign values to variables


```python
a1 = 10   #Assigns value
a1 += 10  #This is same as a1 = a1 + 10
a1 -= 10  #This is same as a1 = a1 - 10
a1 *= 10  #This is same as a1 = a1 * 10
a1 /= 10  #This is same as a1 = a1 / 10
a1 %= 10  #This is same as a1 = a1 % 10
a1 **= 10 #This is same as a1 = a1 ** 10
```

### Operators: Comparison 

It is used to compare two values. It includes equal, not equal, greater than, less than, 
greater than or equal to and less than or equal to.



```python
a2 = 5
b2 = 10
a2 == b2   #a2 is equals to b2 which is False
a2 != b2   #a2 is not equals to b2 which is True
a2 > b2    #a2 is greater than to b2 which is False
a2 < b2    #a2 is lesser than to b2 which is True
a2 >= b2   #a2 is greater than or equal to b2 which is False
a2 <= b2   #a2 is lesser than or than to b2 which is True
```

### Operators: Logical 

It is used to combine statements having conditions. It includes and, or & not statements


```python
a3 = 10
a4 = 15
a3 == 10 and a4 > 8 # and operator which satisfies both the condition and gives True
a3 == 11 or a4 > 8  # or operator which satisfies one of the conditions and gives True
not(a3 == 10) # not operator which reverses the result and gives False for True conditions
```

##  List

- List is a collection of numbers and strings which is ordered and changeable and allows duplicate members.
- List in Python programming is built by setting all the elements inside a square bracket [ ] separated by commas.
- List consists of a string as well as numbers. Indexing, slicing and concatenation from the list can be done.
- Adding element and removing element from the list are some of the works that can be done in a list.


```python
my_list0 = []        # empty list
my_list1 = [2,3,1]   # list with just numbers
my_list2 = ['good','a',100,102.34,90]
                     # list with integers,floats and string
len(my_list1)        # gives length of my_list1 which is 3
len(my_list2)        # gives length of my_list2 which is 5
my_list1[1]          # list indexing with output is 3
my_list2[1:]         # list slicing with output is ['a',100,102.34,90]
my_list1.sort()      # sorts the list with ouput is [1,2,3]
my_list1.reverse()   # reverses the list with output as [1,3,2]
# concatenation with output is [2,3,1, 'good','a',100,102.34,90]
new_list = my_list1 + my_list2 
# changes the index 3 from 'good' into 'b' with new list being [2,3,1,'b','a',100,102.34,90] 
new_list[3]='b' 
# add element on the end of the list with new list being [2,3,1, 'b','a',100,102.34,90, 'six'] 
new_list.append('six') 
# remove last element which is 'six' from the list with new list being [2,3,1, 'b','a',100,102.34,90] 
new_list.pop() 
```

## Tuple

  -  Tuple is a collection which is ordered and unchangeable and also allows duplicate members.
  -  Tuple in Python programming is built by setting all the elements inside a square bracket () separated by commas.
  -  Tuple consists of a string as well as numbers. Indexing and slicing from the tuple can be done.
  -  Difference between list and tuple is that tuple is immutable and list is mutable ie can be changed.


```python
my_tuple = ()         #empty list
my_tuple1 = (2,3,1)   #list with just numbers


len(my_tuple1)        #gives length of my_tuple1 which is 3
my_tuple1[1]          #tuple indexing with output is 3
my_tuple1[1:]         #tuple slicing with output is (3,1)
my_tuple1.count(2)    #counts the number of items having value 2 and output is 1
my_tuple1.index(1)    #gives the index having value 1 with output being 2
```

## Set

  -  Set is a collection which is unordered and unindexed with no duplicate members.
  -  Set in Python programming is built by setting all the elements inside a curly bracket {} separated by commas.
  -  Set consists of a string as well as numbers.


```python
my_set = set()        #empty set
my_set1 = {1,2,3,4}
my_set1.add('a')        #adds additional value a
my_set1.add(1)        #does not adds repeated value 1
```

### Sets: Operations


```python
A = {1,2,3,4}
B = {3,4,5,6}

A.union(B)        #returns union of set A and set B and output is {1, 2, 3, 4, 5, 6}
A.intersection(B) #returns intersection of A and B and output is {3, 4}
A-B               #differece of A and B and output is {1, 2}
A<B               #equivalent to A <= B and A != B and output is False
A>B               #equivalent to A >= B and A != B and output is False
```

## Dictionary

 - Dictionary is a collection which is unordered, changeable and indexed with no duplicate members.
 - Dictionary in Python programming is built by setting all the elements inside a curly bracket with key and values as {key:value} separated by commas.
 - Dictionary consists of a string as well as numbers. Indexing and slicing from the dictionary can be done.


```python
my_dict={'key1':'value1','key2':'value2','key3':'value3'}
my_dict['key1'] #Output is 'value1'

a={'a1':'abc','b1':[3,2,1],'c1':{'d1':12.3}}
a['c1']             #a['c1'] gives {'d1':12.3} 
a['c1']['d1']       #a['c1'] gives {'d1':12.3} and a['c1']['d1'] gives 12.3
#it changes my_dict to {'key1':'Random Value','key2':'value2','key3':'value3'}
my_dict['key1'] = 'Random value'
my_dict.keys()   #it gives all the key i.e. dict_keys(['key1', 'key2', 'key3'])
my_dict.values() #it gives all the key i.e. dict_keys(['Random value', 'value2', 'value3'])
#it gives all the key i.e. dict_items([('key1', 'Random values'), ('key2', 'value2'), ('key3', 'value3')])
my_dict.items() 
    
len(my_dict)     #gives length of my_dict which is 3
```

## Booleans 


```python
a = 10
b = 20
a == b                 #False
a != b                 #True
a > b                  #False
a < b                  #True
a >= b                 #False
a <= b                 #True
a == 10 and b > 8      #True
a == 11 or b > 8       #True
```

## If...elif....else


```python
#Example1

if 4>2:
    print('It is true') #Output is 'It is true'
```


```python
#Example2

word = 'Bank'
if word == 'Mall':
    print('I am in Mall')
elif word == 'Movie':
    print('I am watching a movie')
elif word == 'Bank':
    print('I am depositing money in bank')
else:
    print('I dont know') #Output is 'I am depositing money in bank'
```

##  For loop


```python
#Example 1

mylist = range(10)
list_sum=0
for num in mylist:
    list_sum=list_sum+num
    print(list_sum, end = '  ')  #Outputs are 0  1  3  6  10  15  21  28  36  45  
```


```python
#Example 2

tup=(1,2,3)

for item in tup:
    print(item, end = '  ')   #Outputs are 1 2 3 
```


```python
#Example 3

d={'k1':1,'k2':2,'k3':3}
for item in d:
    print (item, end = '  ')   #Outputs arek1  k2  k3  
```

## While loops


```python
#Example 1

x=0

while x < 1:
    print(f'The current value of x is {x}')
    x+=1
else:
    print('X is not less than 5')

#Output: #L1:The current value of x is 0
         #X L2: X is not less than 5
```

## break/continue/pass

    break: breaks out of the recent nearest loop.
    continue: goes to the top of the nearest loop.
    pass: does nothing at all.


```python
#Example 1

for i in range(3):
    print(i, end = '  ')
    if i>1:
        print('inside', end = '  ')
        continue
    print(i, end = '  ')
print('outside', end = '  ') #Output is : 0  0  1  1  2  2  outside
```


```python
#Example 2

name = 'Sammy'
for letter in name:
    if letter == 'm':
        break
    print(letter) #Output is: s a
```


```python
#Example 3

for i in [0,100,2,5,4]:
    if i==2:
        pass
```

## Functions

Function removes repeatability in code, cleans the code and if any error occurs, you need to correct in only one place


```python
#Example 1: Write a function to check if the word 'dog' is in sentence or not?

def dog(name):
    if 'dog' in name.lower():
        return True
    else:
        return False
```


```python
dog('My Dog ran away') #Output is: True
```


```python
#Example 2: Write a function to check if first letter of the word is vowel?

def word_check(word):
    
    first_letter = word[0]
    
    if first_letter in 'aeiou':
        print('First letter is vowel')
    else:
        print('First letter is consonant')
    return word1
```


```python
word_check('python') #Output is: anker
```


```python
#Example 3: Write a function to returns 5% of the sum of a, b,c and d

def myfunc(a,b,c,d):
    return sum((a,b,c,d))*0.05
```


```python
myfunc(40,60,10,10)
```
