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
     
STRINGS

 think of as a sequence of case sensitive characters

 can compare strings with ==, >, < etc.

 len() is a function used to retrieve the length of the
string in the parentheses

       s = "abc"
        
       len(s)  evaluates to 3
                                        
 square brackets used to perform indexing into a string
to get the value at a certain index/position

s = "abc"

   s[0]  evaluates to "a"

   s[1]  evaluates to "b"
                                        
   s[2]  evaluates to "c"

   s[3]  trying to index out of bounds, error

   s[-1]  evaluates to "c"
                                        
   s[-2]  evaluates to "b"

   s[-3]  evaluates to "a"                                       
                                        
 can slice strings using [start:stop:step]

 if give two numbers, [start:stop], step=1 by default

 you can also omit numbers and leave just colons

s = "abcdefgh"

s[3:6]  evaluates to "def", same as s[3:6:1]

s[3:6:2]  evaluates to "df"

s[::]  evaluates to "abcdefgh", same as s[0:len(s):1]

s[::-1]  evaluates to "hgfedbca", same as s[-1:-(len(s)+1):-1]

s[4:1:-2] evaluates to "ec"
                                        
 strings are “immutable” – cannot be modified
                                    
GUESS-AND-CHECK

 the process below also called exhaustive enumeration
                                        
 given a problem…
                                        
 you are able to guess a value for solution
                                        
 you are able to check if the solution is correct
                                        
 keep guessing until find solution or guessed all values
                                        
GOOD PROGRAMMING
                                        
 more code not necessarily a good thing
                                        
 measure good programmers by the amount of
functionality
                                        
 introduce functions
                                        
 mechanism to achieve decomposition and abstraction

CREATE STRUCTURE with
DECOMPOSITION

 in projector example, separate devices
                                        
 in programming, divide code into modules
                                        
• are self-contained
                                        
• used to break up code
                                        
• intended to be reusable
                                        
• keep code organized
                                        
• keep code coherent
                                        
 this lecture, achieve decomposition with functions
                                        
 in a few weeks, achieve decomposition with classes
                                        
SUPRESS DETAILS with
ABSTRACTION

 in projector example, instructions for how to use it are
sufficient, no need to know how to build one
                                        
 in programming, think of a piece of code as a black box
                                        
• cannot see details
                                        
• do not need to see details
                                        
• do not want to see details
                                        
• hide tedious coding details
                                        
 achieve abstraction with function specifications or
docstrings     
                                        
FUNCTIONS
                                        
 write reusable pieces/chunks of code, called functions
                                        
 functions are not run in a program until they are
“called” or “invoked” in a program
                                        
 function characteristics:
• has a name
                                        
• has parameters (0 or more)
                                        
• has a docstring (optional but recommended)
                                        
• has a body
                                        
• returns something                                       
                                        
VARIABLE SCOPE
                                        
 formal parameter gets bound to the value of
actual parameter when function is called
                                        
 new scope/frame/environment created when enter a function
                                        
 scope is mapping of names to objects
                                        
 Python returns the value None, if no return given
                                        
 represents the absence of a value
                                        
return :
                                        
 return only has meaning
inside a function
                                        
 only one return executed
inside a function
                                        
 code inside function but
after return statement not
executed
                                        
 has a value associated
with it, given to function
caller
                                        
                                        
print:
                                        
 print can be used outside
functions
                                        
 can execute many print
statements inside a function
                                        
 code inside function can be
executed after a print
statement
                                        
 has a value associated with
it, outputted to the console                                        
                                        
 arguments can take on any type, even functions
                                        
SCOPE EXAMPLE:
                                        
 inside a function, can access a variable defined outside
                                        
 inside a function, cannot modify a variable defined
outside -- can using global variables, but frowned upon  
                                        
TUPLES
                                        
 an ordered sequence of elements, can mix element types
                                        
 cannot change element values, immutable
                                        
 represented with parentheses
                                        
t[1:2]   slice tuple, evaluates to ("mit",)
                                        
t[1:3]   slice tuple, evaluates to ("mit",3)
                                        
len(t)   evaluates to 3
                                        
t[1] = 4   gives error, can’t modify object                                        
                                        
 conveniently used to swap variable values   
                                        
 used to return more than one value from a function
                                        
 can iterate over tuples
                                        
LISTS
                                        
 ordered sequence of information, accessible by index
                                        
 a list is denoted by square brackets, []
                                        
 a list contains elements
                                        
• usually homogeneous (ie, all integers)
                                        
• can contain mixed types (not common)
                                        
 list elements can be changed so a list is mutable 
                                        
INDICES AND ORDERING
                                        
a_list = []
                                        
L = [2, 'a', 4, [1,2]]
                                        
len(L)  evaluates to 4
                                        
L[0]  evaluates to 2
                                        
L[2]+1  evaluates to 5
                                        
L[3]  evaluates to [1,2], another list!
                                        
L[4]  gives an error
                                        
i = 2
                                        
L[i-1]  evaluates to ‘a’ since L[1]='a' above 
                                        
CHANGING ELEMENTS
                                        
 lists are mutable!
                                        
 assigning to an element at an index changes the value
                                        
L = [2, 1, 3]
                                        
L[1] = 5
                                        
 L is now [2, 5, 3], note this is the same object L
                                        
ITERATING OVER A LIST
                                        
 compute the sum of elements of a list
                                        
 common pattern, iterate over list elements
                                        
 notice
                                        
• list elements are indexed 0 to len(L)-1
                                        
• range(n) goes from 0 to n-1           
                                        
OPERATIONS ON LISTS - ADD:
                                        
 add elements to end of list with L.append(element)
                                        
 mutates the list!
                                        
L = [2,1,3]
                                        
L.append(5) 
                                        
 L is now [2,1,3,5]
                                        
 what is the dot?
                                        
• lists are Python objects, everything in Python is an object
                                        
• objects have data
                                        
• objects have methods and functions
                                        
• access this information by object_name.do_something()
                                        
 to combine lists together use concatenation, + operator,
to give you a new list
                                        
 mutate list with L.extend(some_list) 
                                        
OPERATIONS ON LISTS -REMOVE:
                                        
 delete element at a specific index with del(L[index])
                                        
 remove element at end of list with L.pop(), returns the
removed element
                                        
 remove a specific element with L.remove(element)
                                        
• looks for the element and removes it
                                        
• if element occurs multiple times, removes first occurrence
                                        
• if element not in list, gives an error 
                                        
CONVERT LISTS TO STRINGS AND BACK:
                                        
 convert string to list with list(s), returns a list with every
character from s an element in L
                                        
 can use s.split(), to split a string on a character parameter,
splits on spaces if called without a parameter
                                        
 use ''.join(L) to turn a list of characters into a string, can
give a character in quotes to add char between every element
                                        
OTHER LIST OPERATIONS

 sort() and sorted()
                                        
 reverse()                                        
                                        
https://docs.python.org/3/tutorial/datastructures.html
                                        
http://www.pythontutor.com/
                                        
LISTS IN MEMORY
                                        
 lists are mutable
                                        
 behave differently than immutable types
                                        
 is an object in memory
                                        
 variable name points to object
                                        
 any variable pointing to that object is affected
                                        
 key phrase to keep in mind when working with lists is side effects

AN ANALOGY
                                        
 attributes of a person
                                        
◦ singer, rich
                                        
 he is known by many names
                                        
 all nicknames point to the same person
                                        
• add new attribute to one nickname …
                                        
• … all his nicknames refer to old attributes AND all new ones
                                        
Justin Bieber singer rich troublemaker
                                        
The Bieb singer rich troublemaker
                                        
JBeebs singer rich troublemaker         
                                        
CLONING A LIST
                                        
 create a new list and copy every element using
                                        
chill = cool[:]
 
SORTING LISTS
 calling sort() mutates the list, returns nothing
                                        
 calling sorted() does not mutate list, must assign result to a variable

LISTS OF LISTS OF LISTS OF….
                                        
 can have nested lists
                                        
 side effects still possible after mutation
                                        
                                        
