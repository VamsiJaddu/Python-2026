function :
  Block of code used to perform specific task .
  def cal(par1, par2):
  return val

 def add(a, b): 
    return a + b

result = add(10, 20)
print(result) o/p:30

def add(a, b):
    print(a + b)

add(5, 3) o/p: 8

def avg():
a = int(input("enter number"))
b = int(input("enter number"))
c = int(input("enter number"))
print ((a+b+c)/3)

def avg() 2 4 6 o/p: 4

Default Parameter Value:

def greet(name , ending="Thank you"):
     print(f"Hi, {name} . Congrats")
     print(ending)
greet("Ganesh") o/p: Hi ganesh thank you
greet("Ganesh", Thanks) o/p: Hi ganesh thanks

lambda function:

lambda arguments_list: expression
s=lambda n:n*n   
print("The Square of 4 is :",s(4))   
print("The Square of 5 is :",s(5))   
    
Output  
The Square of 4 is : 16   
The Square of 5 is : 25  

 filter() function: 
  
 We can use filter() function to filter values from the given sequence based on some 
condition. 
 filter(function,sequence) 
  where function argument is responsible to perform conditional check 
  sequence can be list or tuple or string. 
Q. Program to filter only even numbers from the list by using filter() 
function? 
 
without lambda Function: 
def isEven(x):   
    if x%2==0:   
         return True   
     else:
         return False   
l=[0,5,10,15,20,25,30]   
 l1=list(filter(isEven,l))   
 print(l1)  #[0,10,20,30]   

with lambda Function: 
 l=[0,5,10,15,20,25,30]   
 l1=list(filter(lambda x:x%2==0,l))   
 print(l1)   #[0,10,20,30]   
 l2=list(filter(lambda x:x%2!=0,l))   
 print(l2) #[5,15,25]  

map() function: 
 
 For every element present in the given sequence,apply some functionality and generate 
new element with the required modification.  For this requirement we should go for 
map() function. 
 Eg: For every element present in the list perform double and generate new list of doubles. 
 Syntax:  map(function,sequence) 
 The function can be applied on each element of sequence and generates new sequence. 
 
Eg:  Without lambda 
l=[1,2,3,4,5]   
 def doubleIt(x):   
     return 2*x   
 l1=list(map(doubleIt,l))   
 print(l1) #[2, 4, 6, 8, 10] 
 
with lambda 
 l=[1,2,3,4,5]   
 l1=list(map(lambda x:2*x,l))   
 print(l1)    #[2, 4, 6, 8, 10]   
 
 
Eg 2:   To find square of given numbers 
 l=[1,2,3,4,5]   
 l1=list(map(lambda x:x*x,l))   
 print(l1)       #[1, 4, 9, 16, 25]   
We can apply map() function on multiple lists also.But make sure all list should have same 
length. 
 
Syntax:  map(lambda x,y:x*y,l1,l2)) 
                  x is from l1 and y is from l2 
Eg: 
 l1=[1,2,3,4]   
 l2=[2,3,4,5]   
 l3=list(map(lambda x,y:x*y,l1,l2))   
 print(l3)       #[2, 6, 12, 20]  
 
reduce() function: 
 
reduce() function reduces sequence of elements into a single element by applying the 
specified function. 
 
reduce(function,sequence) 
 
reduce() function present in functools module and hence we should write import 
statement. 
 
Eg: from functools import *   
    l=[10,20,30,40,50]   
    result=reduce(lambda x,y:x+y,l)   
    print(result) # 150  
  
   result=reduce(lambda x,y:x*y,l)   
   print(result)   #12000000   
 
 from functools import *   
 result=reduce(lambda x,y:x+y,range(1,101))   
 print(result)   #5050   
                                                                       
 
18 DURGASOFT, # 202, 2nd Floor, HUDA Maitrivanam, Ameerpet, Hyderabad - 500038,  
 040 – 64 51 27 86, 80 96 96 96 96, 92 46 21 21 43 | www.durgasoft.com 
 
 
Note: 
 In Python every thing is treated as object. 
 Even functions also internally treated as objects only.
