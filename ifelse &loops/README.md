if-elif-else :

if(condition):
   statment1
elif(condition):
    statment2
else:
    statment3

Nested if-else:

age = 34
if(age >= 18):
   if(age >= 75):
      print("you cant drive and licence is cancelled")
    else:  
       print("you can drive")
else:
   print("you are not eligible")

while loop: it prints untill condition is true.

while (condition):
  print("")

Break: it breaks the loop when the idf condition is true.

continue : it jums the current itrtation , when the if condition is true.

for loop:
    num = [1 ,2 , 3 , 4, 2]
    for el in num:
      print(el)

num = [1, 2, 3, 4, 2]
idx = 0
for el in num:
     if el == 4:
        print( "idx", idx)
        break
     idx +=1
 else:
    print("end")    o/p: idx 3 

num = [1, 2, 3, 4, 5]
for el in num:
    print(el)
else:
    print("end")  o/p:1 2 3 4 5 end

 Pass statement: when we want skip that code and working on another function.

  if i < 5:
     pass
   print("hello")  
    

   
