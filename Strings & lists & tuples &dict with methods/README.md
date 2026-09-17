Strings with functions.

   str = "ganesh"
   print(f"My name is {str}")
   print("My name is :", str)
   print("My name is {0}".format(str))
   print("My name is %s" %str)  
   str = 'ganesh'
   str = ''' ganesh '''
* len(str) ----length of string
   a = " "
* len(a) ---o/p: 1
    a = "spd"
    b = "power rangers"
* c = a + b // concentation
    print(c) o/p: spd power rangers
    str = "ganesh"
* str = str.captialize()
    print(str) o/p: Ganesh
* str = str.endswith("esh")
    print(str) o/p:true
  str = "this is a book"
* str.replace("book","pen") o/p: this is a pen
* str.find("word") o/p: prints index of 1st preference
   he's from hyd and his neighbour also from hyd.
* str.count("from") o/p: 2


Lists with functions:

   list = [ 1,3 ,9, 5, 7]
* list.append(4)  add 4
* list.extend([10,11,21])
* list.sort()     asecending order
* list.sort(reverse=true) desceding order
* list.reverse() reverse order
* list.insert(index, ele) list.insert(1,0) o/p: [1 ,0 ,3,9 ,5, 7]
* list.remove(element)
* list.pop(index)

tuple with functions:

   tup =(1 ,)
   print(type(tup)) ..tuple
   tup =(1 ,3 ,5 ,6 , 5)
 * tup.index(element) //tup.index(6)  o/p:3
 * tup.count(elemrnt) //tup.count(5) o/p:2
 * sorted(tup)
 * sorted(tup , reverse=true)
 * min(tup)
 * max(tup)

Dictionaries with function methods:

   student = {
       "name" : "Ranger",
        "subjects" : {
               "phy" : 86 ,
               "chem" : 90 ,
               },
         "age" : 18
    }
 * student.keys() o/p: dict_keys(["name" , "subjects" ])

 * list(student.keys()) o/p:["name" , "subjects" ]
 * list(student.values()) o/p: ["Ranger" , { 'phy': 86 ,'chem' : 90}]
 * student.items() o/p: ('name', 'Ranger'),('subjects',{'phy': 86 ,'chem' : 90}) // return tuples
 * print(student["name"]) o/p: Ranger
   print(student.get("`name")) o/p: Ranger
 * print(student["name2"]) o/p: error
 * prinnt(student.pop("name") removes the name key value
   print(student.get("`name2",defaultvalue)) o/p: none //if default value is there it writes default value instead of none
 * student.update({"grade" : "A"}) 
   o/p: student = {
       "name" : "Ranger",
        "subjects" : {
               "phy" : 86 ,
               "chem" : 90 ,
               },
         "age" : 18 ,
         "grade" : "A"
         
    }

   grociers = {"milk" : 80 , "sugar" : 98 , "milk" : 50 , "vegetables" : 200} o/p: will take milk :50  bcoz it reads from left to right.
set with functions methods: sets are non sequential collection of items. and do not allow duplicates.

set = { 1, 5 ,20 , 45 , 65 , 45}
Here duplicates are removed 
print(set) o/p: {1 , 5 , 20 , 45 ,65}
set = {} ---  empty dictionary
s = set() --- empty set
set.add(10) o/p: {1 , 5 , 10 , 20 , 45 ,65}
set.pop() o/p:{ 1, 10 ,20 , 45 , 65}  
set.remove(20) o/p: { 1, 10 , 45 , 65} out of set number it gives ERROR.
set.discard(45) o/p : {1,5,20,65}  it does not give error .
set.update(range(6)) o/p:  { 0 , 1, 2, 3, 4, 5 ,10 , 45 , 65}
s = {18 , "18"}
s = {20 ,20.0, "20"}  o/p: {20 , "20"} 
here 20 == 20.0 In python assignment operator checks values not datatypes  
s1 ={"Biology", "Maths" , "english" , "chemistry"}
s2 = {"physics", "French" , "maths" , "english" }
Intersection: 
s3 = s1.intersection(s2) // s1 & s2
union:
s3 = s1.intersection(s2) // s1 | s2
s3 = s1.intersection(s2, s4) // s1 | s2 | s4
difference :
days = {"mon" , "Tue" ,"wed", "thu" ,"fri" , "sat" , "sun"}
weekends = {"sat" , "sun"}
weekdays = days - weekends
weekdays = days.difference(weekends)


