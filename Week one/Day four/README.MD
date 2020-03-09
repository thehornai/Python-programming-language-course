##Decision-making

Decision-making is the anticipation of conditions occurring during the execution of a program and specified actions taken according to the conditions.

Decision structures evaluate multiple expressions, which produce TRUE or FALSE as the outcome. You need to determine which action to take and which statements to execute if the outcome is TRUE or FALSE otherwise.

Following is the general form of a typical decision making structure found in most of the programming languages −


Python programming language assumes any non-zero and non-null values as TRUE, and any zero or null values as FALSE value.

Python programming language provides the following types of decision-making statements.


| Sr.No. | Statement & Description |
|--------|-------------------------|
| 1 	 | if statements: An if statement consists of a boolean expression followed by one or more statements. |
| 2	 | if...else statements: An if statement can be followed by an optional else statement, which executes when the boolean expression is FALSE.|
| 3 	 | nested if statements: You can use one if or else if statement inside another if or else if statement(s). |


Let us go through each decision-making statement quickly.

#### Single Statement Suites
If the suite of an if clause consists only of a single line, it may go on the same line as the header statement.

Example
Here is an example of a one-line if clause −

```
#!/usr/bin/python3

var = 100
if ( var  == 100 ) : print ("Value of expression is 100")
print ("Good bye!")
```

Output
When the above code is executed, it produces the following result −
```
Value of expression is 100
Good bye!
```

## Loops

In general, statements are executed sequentially − The first statement in a function is executed first, followed by the second, and so on. There may be a situation when you need to execute a block of code several number of times.

Programming languages provide various control structures that allow more complicated execution paths.

A loop statement allows us to execute a statement or group of statements multiple times. The following diagram illustrates a loop statement −


============ figure goes here =================

Python programming language provides the following types of loops to handle looping requirements.

|Sr.No. | Loop Type & Description |
|-------|-------------------------|
| 1 	| while loop: Repeats a statement or group of statements while a given condition is TRUE. It tests the condition before executing the loop body. |
| 2 	| for loop: Executes a sequence of statements multiple times and abbreviates the code that manages the loop variable.|
| 3	| nested loops: You can use one or more loop inside any another while, or for loop.|


### Loop Control Statements
The Loop control statements change the execution from its normal sequence. When the execution leaves a scope, all automatic objects that were created in that scope are destroyed.

Python supports the following control statements.
|Sr.No.	| Control Statement & Description |
|-------|---------------------------------|
| 1	| break statement: Terminates the loop statement and transfers execution to the statement immediately following the loop.|
| 2	| continue statement: Causes the loop to skip the remainder of its body and immediately retest its condition prior to reiterating.|
| 3	| pass statement: The pass statement in Python is used when a statement is required syntactically but you do not want any command or code to execute.|

Let us go through the loop control statements briefly.

#### Iterator and Generator
Iterator is an object which allows a programmer to traverse through all the elements of a collection, regardless of its specific implementation. In Python, an iterator object implements two methods, iter() and next().

String, List or Tuple objects can be used to create an Iterator.
```
list = [1,2,3,4]
it = iter(list) # this builds an iterator object
print (next(it)) #prints next available element in iterator
Iterator object can be traversed using regular for statement


!usr/bin/python3
for x in it:
   print (x, end=" ")
or using next() function
while True:
   try:
      print (next(it))
   except StopIteration:
      sys.exit() #you have to import sys module for this
```
A **generator** is a function that produces or yields a sequence of values using yield method.

When a generator function is called, it returns a generator object without even beginning execution of the function. When the next() method is called for the first time, the function starts executing until it reaches the yield statement, which returns the yielded value. The yield keeps track i.e. remembers the last execution and the second next() call continues from previous value.

Example
The following example defines a generator, which generates an iterator for all the Fibonacci numbers.

```
#!usr/bin/python3

import sys
def fibonacci(n): #generator function
   a, b, counter = 0, 1, 0
   while True:
      if (counter > n): 
         return
      yield a
      a, b = b, a + b
      counter += 1
f = fibonacci(5) #f is iterator object

while True:
   try:
      print (next(f), end=" ")
   except StopIteration:
      sys.exit()
```