Strings with functions.

   str = "ganesh"
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
   print(student.get("`name2")) o/p: none
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

