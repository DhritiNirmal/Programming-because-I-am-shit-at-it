# Programming-because-I-am-shit-at-it

Course Description
6.0001 Introduction to Computer Science and Programming in Python is intended for students with little or no programming experience. It aims to provide students with an understanding of the role computation can play in solving problems and to help students, regardless of their major, feel justifiably confident of their ability to write small programs that allow them to accomplish useful goals. The class uses the Python 3.5 programming language.

https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-0001-introduction-to-computer-science-and-programming-in-python-fall-2016/lecture-videos/

I'll upload the slides because obviously I do not have patience to watch videos which are this long.


 a program is a sequence of definitions and commands

◦ definitions evaluated

◦ commands executed by Python interpreter in a shell

 commands (statements) instruct interpreter to do
something

 can be typed directly in a shell or stored in a file that
is read into the shell and evaluated

OBJECTS

 programs manipulate data objects

 objects have a type that defines the kinds of things
programs can do to them

◦ Ana is a human so she can walk, speak English, etc.

◦ Chewbacca is a wookie so he can walk, “mwaaarhrhh”, etc.

 objects are

◦ scalar (cannot be subdivided)

◦ non-scalar (have internal structure that can be accessed)

SCALAR OBJECTS

 int – represent integers, ex. 5

 float – represent real numbers, ex. 3.27

 bool – represent Boolean values True and False

 NoneType – special and has one value, None

 can use type() to see the type of an object

TYPE CONVERSIONS (CAST)

 can convert object of one type to another

 float(3) converts integer 3 to float 3.0

 int(3.9) truncates float 3.9 to integer 3

EXPRESSIONS

 combine objects and operators to form expressions

 an expression has a value, which has a type

 syntax for a simple expression

<object> <operator> <object>

OPERATORS ON ints and floats

 i+j  the sum

 i-j  the difference

 i*j  the product

 i/j  division

 i%j  the remainder when i is divided by j

 i**j  i to the power of j

 parentheses used to tell Python to do these
operations first

 operator precedence without parentheses

◦ **

◦ *

◦ /

◦ + and – executed left to right, as appear in expression
  
STRINGS

 letters, special characters, spaces, digits

 enclose in quotation marks or single quotes

  hi = "hello there"
  
 concatenate strings
name = "ana"
greet = hi + name
greeting = hi + " " + name

 do some operations on a string as defined in Python docs
silly = hi + " " + name * 3

INPUT/OUTPUT: input("")

 prints whatever is in the quotes

 user types in something and hits enter

 binds that value to a variable

  text = input("Type anything... ")
  
  print(5*text)

 input gives you a string so must cast if working
with numbers

  num = int(input("Type a number... "))
  
  print(5*num)
  
COMPARISON OPERATORS ON
int, float, string

 i and j are variable names

 comparisons below evaluate to a Boolean

  i > j

  i >= j
  
  i < j

  i <= j

  i == j  equality test, True if i is the same as j

  i != j  inequality test, True if i not the same as j
  
LOGIC OPERATORS ON bools

 a and b are variable names (with Boolean values)

not a  True if a is False
        
        False if a is True

a and b  True if both are True

a or b  True if either or both are True

A     B     A and B     A or B
True True    True        True

True False   False       True

False True   False       True

False False  False       False
 
CONTROL FLOW - BRANCHING

if <condition>:
   
  <expression>
  
  <expression>
...
    
if <condition>:

 <expression>

 <expression>
...

else:

 <expression>
   
 <expression>
...

if <condition>:

<expression>

<expression>
...

elif <condition>:

<expression>

<expression>
...

else:

<expression>

<expression>
...

 <condition> has a value True or False

 evaluate expressions in that block if <condition> is True
  
CONTROL FLOW:

while LOOPS

while <condition>:

<expression>

<expression>
...

 <condition> evaluates to a Boolean
  
 if <condition> is True, do all the steps inside the
while code block

 check <condition> again

 repeat until <condition> is False

CONTROL FLOW: for LOOPS

for <variable> in range(<some_num>):

<expression>

<expression>
...

 each time through the loop, <variable> takes a value

 first time, <variable> starts at the smallest value

 next time, <variable> gets the prev value + 1
  
range(start,stop,step)

 default values are start = 0 and step = 1 and optional

 loop until value is stop - 1 
  
break STATEMENT

 immediately exits whatever loop it is in

 skips remaining expressions in code block

 exits only innermost loop!

while <condition_1>:

while <condition_2>:

  <expression_a>
break
  
   <expression_b>

   <expression_c>
     
