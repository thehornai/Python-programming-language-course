## Variable Types

Variables are nothing but reserved memory locations to store values. It means that when you create a variable, you reserve some space in the memory.

Based on the data type of a variable, the interpreter allocates memory and decides what can be stored in the reserved memory. Therefore, by assigning different data types to the variables, you can store integers, decimals or characters in these variables.

### Assigning Values to Variables
Python variables do not need explicit declaration to reserve memory space. The declaration happens automatically when you assign a value to a variable. The equal sign (=) is used to assign values to variables.

The operand to the left of the = operator is the name of the variable and the operand to the right of the = operator is the value stored in the variable. For example −

```
Live Demo
#!/usr/bin/python3

counter = 100          # An integer assignment
miles   = 1000.0       # A floating point
name    = "John"       # A string

print (counter)
print (miles)
print (name)
```

Here, 100, 1000.0 and "John" are the values assigned to counter, miles, and name variables, respectively. This produces the following result −

```
100
1000.0
John
```

### Multiple Assignment

Python allows you to assign a single value to several variables simultaneously.

For example −
```
a = b = c = 1
```

Here, an integer object is created with the value 1, and all the three variables are assigned to the same memory location. You can also assign multiple objects to multiple variables. For example −

```
a, b, c = 1, 2, "john"
```

Here, two integer objects with values 1 and 2 are assigned to the variables a and b respectively, and one string object with the value "john" is assigned to the variable c.

#### Standard Data Types
The data stored in memory can be of many types. For example, a person's age is stored as a numeric value and his or her address is stored as alphanumeric characters. Python has various standard data types that are used to define the operations possible on them and the storage method for each of them.

Python has five standard data types −

* Numbers
* String
* List
* Tuple
* Dictionary

#### Python Numbers
Number data types store numeric values. Number objects are created when you assign a value to them. For example −

```
var1 = 1
var2 = 10
```

You can also delete the reference to a number object by using the del statement. The syntax of the del statement is −
```
del var1[,var2[,var3[....,varN]]]]
```
You can delete a single object or multiple objects by using the del statement.

For example −
```
del var
del var_a, var_b
```
Python supports three different numerical types −

- int (signed integers)
- float (floating point real values)
- complex (complex numbers)

All integers in Python3 are represented as long integers. Hence, there is no separate number type as long.

##### Examples
Here are some examples of numbers −

|int | float | complex |
|----|-------|---------|
| 10 | 0.0   |  3.14j  |
| 100 |15.20 | 45.j |
| -786 | -21.9 | 9.322e-36j |
| 080 | 32.3+e18 |.876j |
|-0490 | -90. |	-.6545+0J |
|-0x260	| -32.54e100 |	3e+26J |
|0x69 | 70.2-E12 | 4.53e-7j |

A complex number consists of an ordered pair of real floating-point numbers denoted by x + yj, where x and y are real numbers and j is the imaginary unit.

#### Python Strings
Strings in Python are identified as a contiguous set of characters represented in the quotation marks. Python allows either pair of single or double quotes. Subsets of strings can be taken using the slice operator ([ ] and [:] ) with indexes starting at 0 in the beginning of the string and working their way from -1 to the end.

The plus (+) sign is the string concatenation operator and the asterisk (*) is the repetition operator. For example −


```
#!/usr/bin/python3

str = 'Hello World!'

print (str)          # Prints complete string
print (str[0])       # Prints first character of the string
print (str[2:5])     # Prints characters starting from 3rd to 5th
print (str[2:])      # Prints string starting from 3rd character
print (str * 2)      # Prints string two times
print (str + "TEST") # Prints concatenated string
```

This will produce the following result −

```
Hello World!
H
llo
llo World!
Hello World!Hello World!
Hello World!TEST
```

#### Python Lists
Lists are the most versatile of Python's compound data types. A list contains items separated by commas and enclosed within square brackets ([]). To some extent, lists are similar to arrays in C. One of the differences between them is that all the items belonging to a list can be of different data type.

The values stored in a list can be accessed using the slice operator ([ ] and [:]) with indexes starting at 0 in the beginning of the list and working their way to end -1. The plus (+) sign is the list concatenation operator, and the asterisk (*) is the repetition operator. For example −


```
#!/usr/bin/python3

list = [ 'abcd', 786 , 2.23, 'john', 70.2 ]
tinylist = [123, 'john']


print (list)          # Prints complete list
print (list[0])       # Prints first element of the list
print (list[1:3])     # Prints elements starting from 2nd till 3rd 
print (list[2:])      # Prints elements starting from 3rd element
print (tinylist * 2)  # Prints list two times
print (list + tinylist) # Prints concatenated lists
```

This produces the following result −

```
['abcd', 786, 2.23, 'john', 70.200000000000003]
abcd
[786, 2.23]
[2.23, 'john', 70.200000000000003]
[123, 'john', 123, 'john']
['abcd', 786, 2.23, 'john', 70.200000000000003, 123, 'john']
```

#### Python Tuples
A tuple is another sequence data type that is similar to the list. A tuple consists of a number of values separated by commas. Unlike lists, however, tuples are enclosed within parenthesis.

The main difference between lists and tuples are − Lists are enclosed in brackets ( [ ] ) and their elements and size can be changed, while tuples are enclosed in parentheses ( ( ) ) and cannot be updated. Tuples can be thought of as read-only lists. For example −


```
#!/usr/bin/python3

tuple = ( 'abcd', 786 , 2.23, 'john', 70.2  )
tinytuple = (123, 'john')

print (tuple)           # Prints complete tuple
print (tuple[0])        # Prints first element of the tuple
print (tuple[1:3])      # Prints elements starting from 2nd till 3rd 
print (tuple[2:])       # Prints elements starting from 3rd element
print (tinytuple * 2)   # Prints tuple two times
print (tuple + tinytuple) # Prints concatenated tuple
This produces the following result −

('abcd', 786, 2.23, 'john', 70.200000000000003)
abcd
(786, 2.23)
(2.23, 'john', 70.200000000000003)
(123, 'john', 123, 'john')
('abcd', 786, 2.23, 'john', 70.200000000000003, 123, 'john')
```

The following code is invalid with tuple, because we attempted to update a tuple, which is not allowed. Similar case is possible with lists −

```
#!/usr/bin/python3

tuple = ( 'abcd', 786 , 2.23, 'john', 70.2  )
list = [ 'abcd', 786 , 2.23, 'john', 70.2  ]
tuple[2] = 1000    # Invalid syntax with tuple
list[2] = 1000     # Valid syntax with list
```

#### Python Dictionary
Python's dictionaries are kind of hash-table type. They work like associative arrays or hashes found in Perl and consist of key-value pairs. A dictionary key can be almost any Python type, but are usually numbers or strings. Values, on the other hand, can be any arbitrary Python object.

Dictionaries are enclosed by curly braces ({ }) and values can be assigned and accessed using square braces ([]). For example −


```
#!/usr/bin/python3

dict = {}
dict['one'] = "This is one"
dict[2]     = "This is two"

tinydict = {'name': 'john','code':6734, 'dept': 'sales'}

print (dict['one'])       # Prints value for 'one' key
print (dict[2])           # Prints value for 2 key
print (tinydict)          # Prints complete dictionary
print (tinydict.keys())   # Prints all the keys
print (tinydict.values()) # Prints all the values
```

This produces the following result −

```
This is one
This is two
{'name': 'john', 'dept': 'sales', 'code': 6734}
dict_keys(['name', 'dept', 'code'])
dict_values(['john', 'sales', 6734])
```
Dictionaries have no concept of order among the elements. It is incorrect to say that the elements are "out of order"; they are simply unordered.

#### Data Type Conversion
Sometimes, you may need to perform conversions between the built-in types. To convert between types, you simply use the type-names as a function.

There are several built-in functions to perform conversion from one data type to another. These functions return a new object representing the converted value.


| Sr.No. | Function & Description |
|--------|------------------------|
| 1	 | int(x [,base]) Converts x to an integer. The base specifies the base if x is a string.|
| 2	 | float(x) Converts x to a floating-point number. |
| 3	 | complex(real [,imag]) Creates a complex number. |
| 4	 | str(x) Converts object x to a string representation.|
| 5	 | repr(x) Converts object x to an expression string. |
| 6	 | eval(str) Evaluates a string and returns an object. |
| 7	 | tuple(s) Converts s to a tuple. |
| 8	 | list(s) Converts s to a list. |
| 9	 | set(s)  Converts s to a set. |
| 10	 | dict(d) Creates a dictionary. d must be a sequence of (key,value) tuples. |
| 11	 | frozenset(s) Converts s to a frozen set. |
| 12	 | chr(x) Converts an integer to a character. |
| 13	 | unichr(x) Converts an integer to a Unicode character. |
| 14	 | ord(x) Converts a single character to its integer value. |
| 15	 | hex(x) Converts an integer to a hexadecimal string. |
| 16	 | oct(x) Converts an integer to an octal string. |


## Basic Operators

Operators are the constructs, which can manipulate the value of operands. Consider the expression 4 + 5 = 9. Here, 4 and 5 are called the operands and + is called the operator.

#### Types of Operator
Python language supports the following types of operators −

##### Arithmetic Operators
Assume variable a holds the value 10 and variable b holds the value 21, then −
```
+ Addition 
- Subtraction 
* Multiplication 
/ Division 
% Modulus
** Exponent
// Floor Divisio 
```

##### Comparison (Relational) Operators
| symbol | Description |
|--------|-------------|
| ==	 | If the values of two operands are equal, then the condition becomes true. |
| !=	 | If values of two operands are not equal, then condition becomes true. |
| >	 | If the value of left operand is greater than the value of right operand, then condition becomes true. |
| <	 | If the value of left operand is less than the value of right operand, then condition becomes true. |
| >=	 | If the value of left operand is greater than or equal to the value of right operand, then condition becomes true. |
| <=	 | If the value of left operand is less than or equal to the value of right operand, then condition becomes true. |


##### Assignment Operators
```
= Assigns 
+= Add AND	
-= Subtract AND	
*= Multiply AND	 
/= Divide AND
%= Modulus AND	
**= Exponent AND 
//= Floor Division
```
##### Logical Operators
```
and Logical AND	
or Logical OR 
not Logical NOT
```
#### **Bitwise Operators**

##### Membership Operators
Python’s membership operators test for membership in a sequence, such as strings, lists, or tuples. There are two membership operators as explained below −

| Symbol | Description | Example |
|--------|-------------|---------|
|in | Evaluates to true if it finds a variable in the specified sequence and false otherwise. |	x in y, here in results in a 1 if x is a member of sequence y. |
| not in | Evaluates to true if it does not finds a variable in the specified sequence and false otherwise. | x not in y, here not in results in a 1 if x is not a member of sequence y. |

##### Identity Operators
Identity operators compare the memory locations of two objects. There are two Identity operators as explained below −

| Symbol | Desc.. | Example |
|--------|--------|---------|
|is 	 | Evaluates to true if the variables on either side of the operator point to the same object and false otherwise. | x is y, here is results in 1 if id(x) equals id(y). |
|is not  | Evaluates to false if the variables on either side of the operator point to the same object and true otherwise. | x is not y, here is not results in 1 if id(x) is not equal to id(y). |



