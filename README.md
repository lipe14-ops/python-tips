
<img align="center" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" width="100" height="100" />

# 21 python 3.9 quick tips:

## 0. Use lists, tuple, dictionaries, sets comprehensions.
```py
name = [letter for letter in 'Amanda']
print(name) # output: ['A', 'm', 'a', 'n', 'd', 'a']
```
## 1. ALWAYS use explicit variable names and avoid acronyms.
```py
a = 15 # wrong 
age = 15 # right
```
## 2. Play attention at naming.
|use      |fomatting    |exemple         |
|---------|-------------|----------------|
|variables|snake case   | variables_names|
|functions|snake case   | functions_names|
|classes  |Camel Case   | ClassNames     |
|methods  |snake case   | methods_names  |
|constants|constant case| CONSTANTS_NAMES|
|modules  |snake case   | module_name.py |
|package  |flat case    | packagename    |
## 3. Use lambda functions to annonymous functions:
```py
add = lambda y, x: y + x
```
## 4. NEVER write useless comments:
```py
year = 2021 # declaring year variable 
```
## 5. Write imports easy to read.
```py
import math, random, time # wrong

# right way:
import math
import random
import time
```
## 6. Take care about lists, sets, dictionaries and tuples lenght.
```py
transports = ['bus', 'airplane', 'motorbike', 'bike', 'car', 'ship', 'dinosaur'] #wrong

# the right way is:
transports = ['bus',
              'airplane',
              'motorbike',
              'bike',
              'car',
              'ship',
              'dinosaur'
            ]
```
## 7. Look for spaces indentations.
```py
name='John' # wrong
name = 'John'# right
```
## 8. Use to use typing annotations in functions, methods. 
```py
class Person:
    def __init__(self, name: str, age: int) -> None:
        self.name = name
        self.age = age
```
## 9. Always take a space of two lines between functions.
```py
def split_string_by_letter(string: str) -> list:
    return [char for char in string]


def join_list_of_characters(char_list: list) -> str:
    return ''.join(char_list)
```
## 10. Do not forget to use encapsulation:
```py
class Foo:
    public: None
    _protected: None
    __private: None
```
## 11. AVOID to return None:
```py
###### WRONG #####
import datetime

def sleep_time(start_time: int):
    current_time = datetime.datetime.now()
     
    if start_time.year() < current_time:
        return 'sleeping'
    else:
        return None

##### RIGHT WAY #####
import datetime

def sleep_time(start_time: int) -> str:
    current_time = datetime.datetime.now()
     
    if start_time.year() < current_time:
        return 'sleeping'
    else:
        return 'waking up'
```
## 12 Don't forget to use ternary operators.
```py
import datetime

def sleep_time(start_time: int) -> str:
    current_time = datetime.datetime.now()
    return 'sleeping' if start_time < current_time.year() else 'waking up'
```
## 13. Merge dictionaries in one line of code.
```py
mary_name = {'name': 'Mary'}
mary_age = {'age': 20}

mary = mary_name | mary_age # output: {'name':'Mary', 'age': 20}
```
## 14. NEVER use semicolon to break lines.
```py
gender = 'Male';print(gender) # wrong 

# right way:
gender = 'Male'
print(gender)
```
## 15. AVOID to use the `global` keyword.
```py
# DON'T DO IT!!!
def show_all_names(names_list: list) -> None:
    global capitalized_list
    capitalized_list = map(lambda x: x.capitalize(), names_list)
    for name in names_list:
        print(name)
```
use the keyword `return` instead `global`.
## 16. Be organized as possible.
```py
jeny = { 'name':'Jeny','age':17 } # wrong
jeny = {'name':'Jeny',' age':17} # right
```
## 17. Always check if you are in the main file.
```py
if __name__ == '__main__':
    ...
```
## 18. Use designs patterns to large projects.

### some designs patters are: 
1. Facade
2. Observer
3. singleton
4. Factory
5. Proxy

## 19. Repeat strings without loops:
```py
print("hello, world " * 3) # output: hello, world hello, world! hello, world
```

## 20. Switching values of variables:
```py
a = 1
b = 0

a, b = b, a
```
## BONUS!!!
```py
import antigravity
```
look it!!!

### **Author:**
<img width='100' height='100' style="border-radius:50%; padding:15px" src="https://avatars.githubusercontent.com/u/78698099?v=4" /></br>
<a href="https://github.com/lipe14-ops" style='padding: 15px' title="Rocketseat">Filipe Soares :computer:</a>
<p style='padding: 15px'>made with :heart: by <strong>Filipe</strong> :wave: reach me!!!</p>


[![](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](fn697169@gmail.com)
[![](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/filipe_1408/)
