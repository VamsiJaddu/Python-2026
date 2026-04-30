multiple functions , variables, classes are stored in file is called module.

arthametic.py
def add(a,b):
   print(a+b)
def mul(a,b):
   print(a*b)
   x = 10
-------------

using Module in another program

import arthematic
print(arthametic.x)
arthametic.add(20,30)
arthametic.mul(20,30)

using Module as alias

import arthematic as m
print(m.x)
m.add(20,30)
m.mul(20,30)

from...import

from arthematic import x,add
print(x)
add(20,30)

dir() ----inbuilt function
dir(modulename) ....it is used to list the functions, variables etc in particular module.

special variable:

_main_ is the value of the variable , when the program is executed individual.

when the program is executed as module in another program ,then values of the variable is name of the module where it is defined .

# file: test.py

def add(a, b):
    return a + b

if __name__ == "__main__":
    print("Running directly")
    print(add(2, 3))
    o/p:Running directly
        5     

 # main.py
import test o/p: none

random() ===>in between 0 and 1 (not inclusive) 
randint(x,y)   ==>in between x and y ( inclusive) 
uniform(x,y)   ==>  in between x and y ( not inclusive)
   
