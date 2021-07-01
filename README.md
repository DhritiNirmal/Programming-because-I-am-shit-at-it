# Programming-because-I-am-shit-at-it

Course Description
6.0001 Introduction to Computer Science and Programming in Python is intended for students with little or no programming experience. It aims to provide students with an understanding of the role computation can play in solving problems and to help students, regardless of their major, feel justifiably confident of their ability to write small programs that allow them to accomplish useful goals. The class uses the Python 3.5 programming language.

https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-0001-introduction-to-computer-science-and-programming-in-python-fall-2016/lecture-videos/

I'll upload the slides because obviously I do not have patience to watch videos which are these long.


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
