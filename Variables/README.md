Variables:

name = "Ganesh"
age = 23
price = 12.5

print("name") ----o/p: name ...wrong
print(name) ---o/p:Ganesh
print(name , age) ---o/p: Ganesh 23
print("my Name is :" , name) ---my Name is : Ganesh

a = 5
b = a
print(b) ---o/p: 5

a, b, c = 1, 2, 3
o/p:a = 1
    b = 2
    c = 3

a = 5
b = 10
a, b = b, a  
o/p: a = 10
     b = 5
escape sequence:

\n -nextline/new
\t - tab(space)
\' or \" -quotes in btwn lines
\\ - backslash
\

round(sum , 2) --- it gives a value in float with .2 digits o/p : 75.02
pow(2,3) --- 2**3 = 8
abs(-5) --- 5 5 digits from zero
min(list)
max(list)
strip() -- removes space from string
replace(old,new, count) -- it replace into new and if there is char/word more than 1 it will replace  all.
    s1 = "learning python"
    print(s1)
    print(s1.replace("python", "java")
    o/p: learning java
count() --counts occurance of substring in mainstring (char/word)
string.count(substring)
    s1 ="we are learning python. python is fun."
    s2 = "python"
    print(s1.count(s2))
    o/p : 2
startswith() --
string.startswith(substring)
    o/p: true/false
endswith() --
string.endswith(substring)
    o/p: true/false
upper(),lower(),title(),capitalize()
    s1 ="we are learning python. python is fun."
    s1.upper()  --- every char upper
    s1.lower()  --- every char lower
    s1.title()  --- only first char of every word
    s1.capitalize() --- only first char at the line starting.
