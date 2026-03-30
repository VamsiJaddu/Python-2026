Installing of python:python.org 

modules - reuse code available in the form of modules.
pip - is a package manager
"modules" are installed with the help of "pip".

1.built in module - random , math , os , sys

OS module:
To print the contents of directory (files/folders)
Example:
import os
path = "/home/user/Documents"
for file in os.listdir(path): // for entry in os.scandir("."):
    print(file)
    
sys module:
A built-in Python module that provides access to variables and functions used by the Python interpreter to interact with the system
Function Use :
sys.version -	Shows Python version
sys.argv -	Command line arguments
sys.exit() -	Exit program
sys.path	- Module search path

2.external module - flask , pyttsx3(speaks) ,  django , pandas

Comments:
single line: #(ctrl+/)
multiple lines: """     """

Basic Syntax: first.py-->file name
print("Hello World!")
Hello World!

Reserved Words: It represents some meaning or functionality.
 True,False,None
 and, or ,not,is
 if,elif,else
 while,for,break,continue,return,in,yield
 try,except,finally,raise,assert
 import,from,as,class,def,pass,global,nonlocal,lambda,del,with


DATA TYPES:

1. Decimal Form (Base 10)

Uses 10 digits: 0–9

This is the normal number system we use daily.

Example: 125₁₀

2. Binary Form (Base 2)

Uses 2 digits: 0(OFF) and 1(ON) in electronics circuits

This is the language of computers.

Example: 1011₂

Decimal 5 = Binary 101

Binary Place Values

Binary uses base 2, so place values are powers of 2:

Position	2²	2¹	2⁰
Value	    4	  2	  1

Binary number: 1 0 1

3. Octal Form (Base 8)

 1 oct = 3 binary digits (111)  

Uses 8 digits: 0–7

Shorter way to represent binary numbers.

Example: 17₈

Binary 111 = Octal 7

4. Hexadecimal Form (Base 16)

1 Hex digit = 4 Binary digits (1111)

Uses 16 symbols: 0–9 and A–F

A=10, B=11, C=12, D=13, E=14, F=15

Commonly used in memory addresses and colors.

Example: 2F₁₆

Decimal 15 = Hex F

| System      | Base | Digits Used | Example |
| ----------- | ---- | ----------- | ------- |
| Decimal     | 10   | 0–9         | 125     |
| Binary      | 2    | 0–1         | 1011    |
| Octal       | 8    | 0–7         | 17      |
| Hexadecimal | 16   | 0–9, A–F    | 2F      |

5. type() - is to check the type of the variable
6. id()   - is to check the address of the object
7. print() - to print the value
8. bin() - to convert from any base to binary
9. oct() - to convert from any base to octal
10. hex() - to convert from any base to hex decimal.

11.complex datatype:
        c = a+bj
          a---real part
          b---imaginary part
          j--- imaginary unit

12.string:
    str = "" or '' ---> single 
    str = '''  
            multiple line 
           '''
           
13. slicing:
   str = "python" 

     -6-5-4-3-2-1
      p y t h o n
      0 1 2 3 4 5
     str[0] p
     str[:] python
     str[0:40] python
     str[1:] ython
     str[:4] pyth

14. fundamental Datatypes and Immutable:  
       Python uses Integer Interning (Caching)
       Python reuses memory for small integers (typically from -5 to 256)
       No caching for complex numbers
          a = 10
          b = 10
          id(a)  → same    (id == function)
          id(b)  → same
          a is b → True  (is = operator)
    // Python stores only one object 10 in memory. Both a and b point to the same memory location.

15. Byte data type:
      x = [10 , 20, 30 , 40]
      bytes(x)
      b = bytes([10, 20, 30, 40])
      bytes() converts a list of integers → bytes object . Each value must be in range 0 to 255   
      x = [10, 20, 30, 40]
      b = bytes(x)
        type(b)        # bytes
        print(b[0])    # 10
        print(b[-1])   # 40
        for i in b:
            print(i) : o/p : 10 20 30 40
      Once we creates bytes data type value, we cannot change its values,otherwise we will get TypeError.

16. Bytearray data type :
       bytearray is exactly same as bytes data type except that its elements can be modified.
        x = [10, 20, 30, 40]
        b = bytearray(x)
        print(b[0])    # 10
        print(b[-1])   # 40
        b[0] = 100
        for i in b:
            print(i) : o/p : 100 20 30 40
      
17.list :
      you can store any value , duplicates, change.
        list = [10, 10.5 , "example", 10]
        list = list.append("spd") o/p: [10, 10.5 , "example", 10, 'spd']
        list = list.remove(10) o/p: [10.5 , "example", 10, 'spd']  only first predence is removed.
        list = list.pop(0) o/p: ["example", 10, 'spd']
        list2 = list*2 o/p :  ["example", 10, 'spd', "example", 10, 'spd']
        
18. tuple :
        you  can store the values , but you cant change.Read only        
        tuple = (10, 10.5 , "example", 10)

19. Range data type:
         you cant change .
    Form-1: range(10)
            generate numbers from 0 to 9
            Eg:
            r=range(10)
            for i in r : print(i) 0 to 9
    Form-2: range(10,20)
             generate numbers from 10 to 19
             r = range(10,20)
             for i in r : print(i) 10 to 19
    form 3 : range(10,20,2)
            2 means increment value
            r = range(10,20,2)
            for i in r : print(i) 10,12,14,16,18
        We can access elements present in the range Data Type by using index.
        r=range(10,20)
        r[0]==>10
        r[15]==>IndexError: range object index out of range
        We cannot modify the values of range data type
        Eg:
        r[0]=100
        TypeError: 'range' object does not support item assignment
        We can create a list of values with range data type
        Eg:
        l = list(range(10))
        l=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

  20. set datatype:
             you can store any value ,duplicates are removed , you can change add, remove values .
             s = {10, 20, 10, 30}
                 print(s) o/p: {10, 20, 30}
              s = {10, 20}
                s.add(30)
                print(s) o/p: {10,20, 30}

  21. frozenset data type:
                it is same as set but here cant add, remove. Only read.

  22. Dict data type:
        A dictionary stores data in key : value pairs.
            Keys → unique 
            Values → can be anything 
            Mutable (can change)
          d = {"name": "Vamsi"}
            d["age"] = 25        # add
            d["name"] = "Krishna" # update
            print(d) o/p: {'name': 'Krishna', 'age': 25}
