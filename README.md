# OOP
OOP 
23/04/2020
Computer program:                                        Add two numbers
solves problems using a computer
Input:                                                                    2 numbers num1 and num2
Functionality/algorithm:                               add functionality to add num1 and num2
output: returned value, print
Inputs and Expected Output
2,0                          2              Pass
2,1                          3              Pass
2,2                          4             Pass
-1,3                        2
-3,-5                       -8


Function to solve problem:
re-usability
Input arguments, functionName, output
Inputs & Expected Output

Test Cases get executed every time you run an assignment in Lex
Test cases test our functions automatically
Test case has input, expected output
it executes the function and checks if expected output is equal to actual output. If it is, then test case Pass else Fail
Assessment:
0. A set of Test cases covering all the business scenarios over your solution  
1.Test cases for functions you will write and submit
2. The test cases will be executed on your submitted code
3. Each test case is allocated a mark/score
4. Your final score is the marks of all the test cases that have passed
5. If all test cases pass, you get full marks

Hands On assessment:
PF: programming Fundamentals you get one question in which you need to code inside one function only

OOP
re-usability
Separation of concern: example: packages

Objects: 1. they have data/characteristic/Attribute/Properties
                value of attributes will help in uniquely defining objects
                Example: Product: productId,productName
                                Mobile: price, brand
                                Shoe: price,material
                2. also they have behavior/methods(functionality)
                Example: Mobile: purchare and return
                associated




Mobile: (1000,"Samsung")
(10000,"Apple")
(20000,"Asus")
Mobile class: description of properties: price, brand
                                behavior: purchase, return
value of properties of a class will help create unique objects

Class keyword define a class: class ClassName:
create object:"<ClassName>()"
this way of creating objects calls the default __init__()

when object is created, unique Id is created, unique memory location to store value of attributes

reference variable:
holds the reference to the object
id(<reference variable name>): returns unique ID

after object is created, to create attribute:
reference_variable.attribute_name=value
Warning: We are programmers are barred/not allowed to create attributes after object is created in enterprise application

Can we have separate attributes for specific objects?

Access value of attributes inside an object:
reference_variable.attribute_name

ref_var1 = ref_var2
ref_var1 and ref_var2 will point to the same memory location
OR
ref_var1 will also start pointing to the memory location of ref_var2


How to define attributes while defining the class itself?
Best practice is to define the attributes while defining the class itself
__init__/ initializer method/ constructor
__init__ special method to define,create and provide values to attributes of the class

__init__ method is present in all classes by default.
to define and create attributes of the class
__init__ will always have self as first parameter
To create attribute: self.<attributeName>=Initial value


METHODS:
functions present inside class
all methods will have at least self as the first parameter
self refers to the calling/current object


24/04/2020
When object is created:
The object is initialzed by calling __init__ method/Constructor
If __init__ is not defined, default __init__() (parameterlesss constructor) is called which does nothing

Create object <ClassName>(<pass values for __init__>) and store it in reference variable
Reference variables stores the momory location of an object:"It can refer to an object"

Class needs to defines and initialize its attributes/properties/Instance variables during class definition
We can do that by using the __init__
1. __init__ helps initialize an object of a class
2. When object is created, __init__ method is invoked
3. self with dot operator helps in creating attributes and assigning initial values to them self.<attribute_name>=<value>


parameterless contructor(__init__): special METHOD
METHOD: functions inside a Class that have one default parameter always named as self
SELF: calling/current object
self with dot operator helps in creating attributes and assigning initial values to them
self.<attribute_name>=<value>
IMP: all methods should have at least one parameter, That parameter becomes the calling/current object. For convenience we should name it as self.
But it can be named anything


**When does an attribute error happen?
#Accessing a non existing attribute
you can access an attribute by <reference var Name>.<attribute_name>
If you write the name of an attribute that does not exist, then you get attribute error





Parameterized constructor/Initializer
1. Help us to set initial values to the attributes when the object gets created
2. __init__ has one or more than one parameter other than self
You pass only the exact number of values as there are parameters/argumements __init__

When object is created:
The object is initialzed by calling __init__ method/Constructor
If __init__ is not defined, default __init__() (parameterlesss constructor) is called which does nothing

Create object <ClassName>(<pass values for __init__>) and store it in reference variable
Reference variables stores the momory location of an object:"It can refer to an object"

Class needs to defines and initialize its attributes/properties/Instance variables during class definition
We can do that by using the __init__
1. __init__ helps initialize an object of a class
2. When object is created, __init__ method is invoked
3. self with dot operator helps in creating attributes and assigning initial values to them self.<attribute_name>=<value>


parameterless contructor(__init__): special METHOD
METHOD: functions inside a Class that have one default parameter always named as self
Methods can access the attributes of the current object by self.<attributeName>
To call a method: <reference_var_name>.<methodName>(argument values is preent)
Inside method we refer to self as the CALLING object. 
The calling object is the one who called/invoked the method using dot operator
A method exists only because an object(using its reference variable name) has called it


SELF: calling/current object
self with dot operator helps in creating attributes and assigning initial values to them
self.<attribute_name>=<value>
IMP: all methods should have at least one parameter, That parameter becomes the calling/current object. For convenience we should name it as self.
But it can be named anything


**When does an attribute error happen?
#Accessing a non existing attribute
you can access an attribute by <reference var Name>.<attribute_name>
If you write the name of an attribute that does not exist, then you get attribute error


Parameterized constructor/Initializer
1. Help us to set initial values to the attributes when the object gets created
2. __init__ has one or more than one parameter other than self
You pass only the exact number of values as there are parameters/argumements __init__

Local variiables inside Method:
Local variables lifetime: limited inside the function

__str__ : special method
1. It is by default present in all Objects(Class). By default the output has the format:<__main__.Shoe object at 0x7f16861f6ba8> <package_name>.<Class Name> at Memory Location(fake)
2. It gets invoked everytime you print an object
3. You can always override the default __str__ method in a Class by defining it again(Method Overriding)


Class: Product, Shoe, Mobile do you see any relation between these classes?
Shoe and Mobile are Products

Concepts and Relations in OOP:
Abstraction
Encapsulation
Inheritance
Aggregation

Abstraction:
------------
This concept in OOP has been copied from Fucntional Programming
All functions including methods demonstrate Abstraction.
You need not worry about the implementation of the function/method when you invoke(call) it
Encapsulation:
------------- 
Restricting access to attributes of a class
Make attributes marked as Public or Private
If private, the attribute will not be accessible outside the class defining
To mark attribute as private: __AttributeName(adding a double underscore in front)
Python implements encapsulation by changing the name of the private attribute from __AttributeName to _ClassName__AttributeName
private: private access specifier __AttributeName (-)
public: public access specifier: AttributeName (+)

To access private attributes we can use setter and getter methods:
They are methods just following a Naming standard:
get_attributeName: getter
set_AttributeName: setter


Python gives the ability to create instance variables even after the object is created. <reference_var_Name>.<newAttributeName>=value


27/04/2020
Objects
Class: RecipeCard/Blueprint to create object
Objects have Attributes and Methods
Attributes: Properties, Instance variables
Methods: Behaviors(functionality)
fucntions present inside class and always have self(calling/current object) as thier first parameter
Attribute Error: Acces a non existing attribute
Python allows you to create attributes after object has been created
self: current/ calling object
__init__:special method:
1. __init__ initializer method, constructor
2. Two types:parameterless; parameterized
3. __init__ helps us to create object, it gets called whnever object is created. It also helps us to initialize values for attributes(optional)
METHODS
1. methods can be invoked or called only by an object by: <reference_varName>.methodName(<argument values>)

**C1=C2(customer object)
C1 will start pointing to the object where C1 is is pointing to

--------------------------------------
Day 2
Passing values for parameters/arguments of a function/method happen in two ways:
pass by value
pass by reference

PASS BY REFERENCE
def change_price(mobile_obj):
mob1=Mobile(1000, "Apple")

change_price(mob1)
mobile_obj=mob1
The reference of mob1 is being passed to mobile_obj
>>Both mobile_obj and mob1 will now point to the same object
pass by reference happens when we try to pass objects through thier reference variables
List are objects, they will go for pass by reference


PASS BY VALUE
when only value is passed. The argument passed and the parameter/input argument have no relation. Only value is passed
Numbers go for pass by value

DICT
define by dict_name = {key1:value1,key2,value2...}
dict_name = {}(Empty dict)
dict_name[key] = value (Add key value pair to dict)

Hardcoding inside classes is not allowed


STATIC

Need for static?
We need a common space where we can define attributes which are common for all objects

How to create static variables of a class?
Variables are defined directly inside the class and not inside __init__

To ACCESS/UPDATE a Static variable you can use ClassName.<staticVarName>
static variables belong to a class and not individual object

To make static variables are private put __before the name

STATIC METHODS:
meant to work only with static variables that require Class Name itself and do not require self
1. Special methods inside class that do not have self
2. These methods have to be annotated with @staticmethod to make them static

