# python-basics_3
Basics of python in Cpt Classes under the Guidance of CODEGNAN in NRIIT
#Arithmetic Operations
num1=int(input())
num2=int(input())
total=num1+num2
print(total)
///
#Add Strings
str1=input("enter a name")
str2=input("enter a name")
fullname=str1+str2
print(fullname)
///
#float datatype sample
num1=float(input("enter a float value"))
num2=float(input("enter a float value"))
print("addition:",num1+num2)
///
#Operations performend by string 
s=str(input("enter a string:"))
print(s)
print(len(s))
print(s.upper())
print(s.lower())
print(s[2:5])
print(s[::-2])
///
#List Operations
fruits=['apple','kiwi','orange']
print(fruits)
fruits.append('banana')#insert
print(fruits)
fruits.remove('kiwi')#delete
print(fruits)
print(fruits[0])
print(fruits[-3])
