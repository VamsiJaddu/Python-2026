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
