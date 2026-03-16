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
   >>>str[0] p
   >>>str[:] python
   >>>str[0:40] python
   >>>str[1:] ython
   >>>str[:4] pyth

14.



