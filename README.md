# python-basics_2
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
///
# Python_basics-CPT-4
Basics of Python which includes the topic "TUPLE","DICTIONARY"
///
#list with in tuple
student=("vijay",[25,50,90],['maths' , 'physics' , 'chemistry'])
print(student[1])
print(student[0])
print(student[2])
print(student[2][1])
print(student[2][2])
print(student[2][0])
OUTPUT:
[25, 50, 90]
vijay
['maths', 'physics', 'chemistry']
physics
chemistry
maths
///
#tuple sample
info= ("Sashi",20,'student')
print(info[1],info[2],info[0])
#print(info.append(salary))
print(info[-2])
print(len(info))
print(info*2)
print(info+(3,4)) #tuple is added as info not as nested tuple(append operation)
print(info+('college fees','42500'))#append operation
OUTPUT:
20 student Sashi
20
3
('Sashi', 20, 'student', 'Sashi', 20, 'student')
('Sashi', 20, 'student', 3, 4)
('Sashi', 20, 'student', 'college fees', '42500')
///
#nested tuple
nest=((1,2),(3,4),(5,6))
print(nest[0])
print(nest[1][0])
print(nest[2][0])
OUTPUT:
(1, 2)
3
5
///
#DICTIONARY OPERATIONS.....
person={'name':'sashi','age':20,'city':'vijayawada'}
print(person)
print("accessing the person age:")
person["age"]= 25
print(person)
print("Adding the person email Address")
print(person)
person["email"]='sashigangadhar010605@gmail.com'
print(person)
print("deleting the city ")
del person['city']
print(person)
print("All Keys and values")
print(person.keys())
print(person.values())
print(person.items())
print(person.get("age"))
OUTPUT:
{'name': 'sashi', 'age': 20, 'city': 'vijayawada'}
accessing the person age:
{'name': 'sashi', 'age': 25, 'city': 'vijayawada'}
Adding the person email Address
{'name': 'sashi', 'age': 25, 'city': 'vijayawada'}
{'name': 'sashi', 'age': 25, 'city': 'vijayawada', 'email': 'sashigangadhar010605@gmail.com'}
deleting the city 
{'name': 'sashi', 'age': 25, 'email': 'sashigangadhar010605@gmail.com'}
All Keys and values
dict_keys(['name', 'age', 'email'])
dict_values(['sashi', 25, 'sashigangadhar010605@gmail.com'])
dict_items([('name', 'sashi'), ('age', 25), ('email', 'sashigangadhar010605@gmail.com')])
25
///
#nested Dictionary
info={
    'sashi':{"fees":42500,"perks":5000},
    'prashu':{"fees":42500,"perks":3000},
}
print(info['prashu']['perks'])
print(info['sashi']['perks'])
print(info['prashu']['fees'])
print(info['sashi']['fees'])
OUTPUT:
3000
5000
42500
42500
///
#dict with tuples as keys
location={
    (40.278,-66.020):'New York',
    (30.524,-54.745):'Melbourne'}
print(location[(40.278,-66.020)])
print(location[(30.524,-54.745)])
OUTPUT:
New York
Melbourne
///
#accessing value from key: 
info={'name':'india','number':123}
v= 'india'
for key,value in info.items():
    if value==v:
        print(f"key for value'{v}':{key}")
OUTPUT:
key for value'india':name
///
#SET OPERATIONS.........
my_set={1,2,3,4,5,6}
print(my_set)
print("add and remov values")
my_set.add(7)
print(my_set)
my_set.remove(2)
print(my_set)
my_set.discard(6)
print(my_set)
print("Membership Check")
print(1 in my_set)
print(10 in my_set)
OUTPUT:
{1, 2, 3, 4, 5, 6}
add and remov values
{1, 2, 3, 4, 5, 6, 7}
{1, 3, 4, 5, 6, 7}
{1, 3, 4, 5, 7}
Membership Check
True
False
///
#Operations
print("union")
a={1,2,3}
b={3,4,5}
print(a.union(b))
print("intersection")
print(a.intersection(b))
print("difference")
print(a.difference(b))
print("symmetricdifference")
print(a.symmetric_difference(b))
OUTPUT:
union
{1, 2, 3, 4, 5}
intersection
{3}
difference
{1, 2}
symmetricdifference
{1, 2, 4, 5}
///
#REMOVING DUPLICATE VALUES IN SET
nums=[1,2,2,3]
unique= set(nums)#always duplicate num is 1st one here index of 1 is duplicate and index of 2 is latest
print(unique)
OUTPUT:
{1, 2, 3}
///
# TYPES OF SUBSET OPERATIONS......
a={1,2}
b={1,2,3,4,5}
print(a.issubset(b))
print(b.issubset(a))
print(a<=b)#improper subset
print(a<b)#proper subset
print(a>=b)
print(b>a)
output:
True
False
True
True
False
True
///
#by using conditional operators
a={1,2}
b={1,2,3,4,5}
print("subset or not:",a<=b)#subset
print("proper subset or not:",a<b)#subset
print("proper subset or not:",b<a)#subset
print("subset or not:",b<=a)#subset
print("superset or not:",a>=b)#super set
print("proper superset:",b>a)#super set
print("superset or not:",b>=a)#super set
print("proper superset:",a>b)#super set
OUTPUT:
Selection deleted
#by using conditional operators
a={1,2}
b={1,2,3,4,5}
print("subset or not:",a<=b)#subset
print("proper subset or not:",a<b)#subset
print("proper subset or not:",b<a)#subset
print("subset or not:",b<=a)#subset
print("superset or not:",a>=b)#super set
print("proper superset:",b>a)#super set
print("superset or not:",b>=a)#super set
print("proper superset:",a>b)#super set

subset or not: True
proper subset or not: True
proper subset or not: False
subset or not: False
superset or not: False
proper superset: True
superset or not: True
proper superset: False
///
