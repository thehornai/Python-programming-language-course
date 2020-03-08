## Python Tutorial

Python is a general-purpose interpreted, interactive, object-oriented, and high-level programming language. It was created by Guido van Rossum during 1985- 1990. Like Perl, Python source code is also available under the GNU General Public License (GPL). Python is named after a TV Show called ëMonty Pythonís Flying Circusí and not after Python-the snake.

Python 3.0 was released in 2008. Although this version is supposed to be backward incompatibles, later on many of its important features have been backported to be compatible with version 2.7. This tutorial gives enough understanding on Python 3 version programming language.
### Why to Learn Python?
Python is a high-level, interpreted, interactive and object-oriented scripting language. Python is designed to be highly readable. It uses English keywords frequently where as other languages use punctuation, and it has fewer syntactical constructions than other languages.

Python is a MUST for students and working professionals to become a great Software Engineer specially when they are working in Web Development Domain. I will list down some of the key advantages of learning Python:

* __Python is Interpreted__ − Python is processed at runtime by the interpreter. You do not need to compile your program before executing it. This is similar to PERL and PHP.

* __Python is Interactive__ − You can actually sit at a Python prompt and interact with the interpreter directly to write your programs.

* __Python is Object-Oriented__ − Python supports Object-Oriented style or technique of programming that encapsulates code within objects.

* __Python is a Beginner's Language__ − Python is a great language for the beginner-level programmers and supports the development of a wide range of applications from simple text processing to WWW browsers to games.

### Characteristics of Python
Following are important characteristics of python −

- It supports functional and structured programming methods as well as OOP.

- It can be used as a scripting language or can be compiled to byte-code for building large applications.

- It provides very high-level dynamic data types and supports dynamic type checking.

- It supports automatic garbage collection.

- It can be easily integrated with C, C++, COM, ActiveX, CORBA, and Java.

### Hello World using Python.
Just to give you a little excitement about Python, I'm going to give you a small conventional Python Hello World program, You can try it using Demo link.

```python
print "Hello, Python!"
```

### Applications of Python
As mentioned before, Python is one of the most widely used language over the web. I'm going to list few of them here:

* Easy-to-learn − Python has few keywords, simple structure, and a clearly defined syntax. This allows the student to pick up the language quickly.

* Easy-to-read − Python code is more clearly defined and visible to the eyes.

* Easy-to-maintain − Python's source code is fairly easy-to-maintain.

* A broad standard library − Python's bulk of the library is very portable and cross-platform compatible on UNIX, Windows, and Macintosh.

* Interactive Mode − Python has support for an interactive mode which allows interactive testing and debugging of snippets of code.

* Portable − Python can run on a wide variety of hardware platforms and has the same interface on all platforms.

* Extendable − You can add low-level modules to the Python interpreter. These modules enable programmers to add to or customize their tools to be more efficient.

* Databases − Python provides interfaces to all major commercial databases.

* GUI Programming − Python supports GUI applications that can be created and ported to many system calls, libraries and windows systems, such as Windows MFC, Macintosh, and the X Window system of Unix.

* Scalable − Python provides a better structure and support for large programs than shell scripting.

### Audience
This tutorial is designed for software programmers who want to upgrade their Python skills to Python. This tutorial can also be used to learn Python programming language from scratch.

### Prerequisites
You should have a basic understanding of Computer Programming terminologies. A basic understanding of any of the programming languages is a plus.



Python is available for Windows, Mac OS and most of the flavors of Linux operating system.

### Local Environment Setup
Open a terminal window and type "python" to find out if it is already installed and which version is installed.

### Getting Python
#### Windows platform
Binaries of latest version of Python 3 (Python 3.5.1) are available on this download page

The following different installation options are available.

 * Windows x86-64 embeddable zip file
 * Windows x86-64 executable installer
 * Windows x86-64 web-based installer
 * Windows x86 embeddable zip file
 * Windows x86 executable installer
 * Windows x86 web-based installer
**Note** − In order to install Python 3.5.1, minimum OS requirements are Windows 7 with SP1. For versions 3.0 to 3.4.x Windows XP is acceptable.

#### Linux platform
Different flavors of Linux use different package managers for installation of new packages.

On Ubuntu Linux, Python is installed using the following command from the terminal.
```
$sudo apt-get install python3-minimal
```
Installation from source

Download Gzipped source tarball from Python's download URL - https://www.python.org/ftp/python/3.5.1/Python-3.5.1.tgz

```
Extract the tarball
tar xvfz Python-3.5.1.tgz
Configure and Install:
cd Python-3.5.1
./configure --prefix = /opt/python3.5.1
make  
sudo make install
```


The most up-to-date and current source code, binaries, documentation, news, etc., is available on the official website of Python −

**Python Official Website** − https://www.python.org/

You can download Python documentation from the following site. The documentation is available in HTML, PDF and PostScript formats.

**Python Documentation Website** − www.python.org/doc/


#### Setting Path at Unix/Linux
To add the Python directory to the path for a particular session in Unix −

In the csh shell − type setenv PATH "$PATH:/usr/local/bin/python3" and press Enter.

In the bash shell (Linux) − type export PYTHONPATH=/usr/local/bin/python3.4 and press Enter.

In the sh or ksh shell − type PATH = "$PATH:/usr/local/bin/python3" and press Enter.

Note − /usr/local/bin/python3 is the path of the Python directory.

#### Setting Path at Windows
To add the Python directory to the path for a particular session in Windows −

At the command prompt − type path %path%;C:\Python and press Enter.

Note − C:\Python is the path of the Python directory

#### Python Environment Variables
Here are important environment variables, which are recognized by Python −

| Sr.No. | Variable & Description |
|--------|------------------------|
| 1 | **PYTHONPATH** It has a role similar to PATH. This variable tells the Python interpreter where to locate the module files imported into a program. It should include the Python source library directory and the directories containing Python source code. PYTHONPATH is sometimes preset by the Python installer.|
| 2 | **PYTHONSTARTUP** It contains the path of an initialization file containing Python source code. It is executed every time you start the interpreter. It is named as .pythonrc.py in Unix and it contains commands that load utilities or modify PYTHONPATH.|
| 3 | **PYTHONCASEOK** It is used in Windows to instruct Python to find the first case-insensitive match in an import statement. Set this variable to any value to activate it.|
| 4 | **PYTHONHOME** It is an alternative module search path. It is usually embedded in the PYTHONSTARTUP or PYTHONPATH directories to make switching module libraries easy.|


### Python Identifiers
A Python identifier is a name used to identify a variable, function, class, module or other object. An identifier starts with a letter A to Z or a to z or an underscore (_) followed by zero or more letters, underscores and digits (0 to 9).

Python does not allow punctuation characters such as @, $, and % within identifiers. Python is a case sensitive programming language. Thus, **Manpower** and **manpower** are two different identifiers in Python.

Here are naming conventions for Python identifiers −

Class names start with an uppercase letter. All other identifiers start with a lowercase letter.

Starting an identifier with a single leading underscore indicates that the identifier is private.

Starting an identifier with two leading underscores indicates a strong private identifier.

If the identifier also ends with two trailing underscores, the identifier is a language-defined special name.

### Reserved Words
The following list shows the Python keywords. These are reserved words and you cannot use them as constants or variables or any other identifier names. All the Python keywords contain lowercase letters only.

| and | exec | not |
|as | finally | or |
|assert	for	pass
|break | from | print|
|class | global | raise |
|continue | if | return |
|def | import | try|
|del | in | while |
|elif | is | with|
|else | lambda | yield|
|except	|

### Lines and Indentation
Python does not use braces({}) to indicate blocks of code for class and function definitions or flow control. Blocks of code are denoted by line indentation, which is rigidly enforced.

The number of spaces in the indentation is variable, but all statements within the block must be indented the same amount. For example −

```
if True:
   print ("True")

else:
   print ("False")
```
However, the following block generates an error −

```
if True:
   print ("Answer")
   print ("True")

else:
   print "(Answer")
   print ("False")
```
Thus, in Python all the continuous lines indented with the same number of spaces would form a block. The following example has various statement blocks −

Note − Do not try to understand the logic at this point of time. Just make sure you understood the various blocks even if they are without braces.

#!/usr/bin/python3

import sys

try:
   # open file stream
   file = open(file_name, "w")

except IOError:
   print ("There was an error writing to", file_name)
   sys.exit()
print ("Enter '", file_finish,)
print "' When finished"

while file_text != file_finish:
   file_text = raw_input("Enter text: ")
   
   if file_text == file_finish:
      # close the file
	  file.close
      break
   file.write(file_text)
   file.write("\n")
file.close()
file_name = input("Enter filename: ")

if len(file_name) == 0:
   print ("Next time please enter something")
   sys.exit()

try:
   file = open(file_name, "r")

except IOError:
   print ("There was an error reading file")
   sys.exit()
file_text = file.read()
file.close()
print (file_text)
Multi-Line Statements
Statements in Python typically end with a new line. Python, however, allows the use of the line continuation character (\) to denote that the line should continue. For example −

total = item_one + \
   item_two + \
   item_three
The statements contained within the [], {}, or () brackets do not need to use the line continuation character. For example −

days = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday']
Quotation in Python
Python accepts single ('), double (") and triple (''' or """) quotes to denote string literals, as long as the same type of quote starts and ends the string.

The triple quotes are used to span the string across multiple lines. For example, all the following are legal −

word = 'word'
sentence = "This is a sentence."
paragraph = """This is a paragraph. It is
made up of multiple lines and sentences."""
Comments in Python
A hash sign (#) that is not inside a string literal is the beginning of a comment. All characters after the #, up to the end of the physical line, are part of the comment and the Python interpreter ignores them.

Live Demo
#!/usr/bin/python3

# First comment
print ("Hello, Python!") # second comment
This produces the following result −

Hello, Python!
You can type a comment on the same line after a statement or expression −

name = "Madisetti" # This is again comment
You can comment multiple lines as follows −

# This is a comment.
# This is a comment, too.
# This is a comment, too.
# I said that already.
Following triple-quoted string is also ignored by Python interpreter and can be used as a multiline comments:

'''
This is a multiline
comment.
'''
Using Blank Lines
A line containing only whitespace, possibly with a comment, is known as a blank line and Python totally ignores it.

In an interactive interpreter session, you must enter an empty physical line to terminate a multiline statement.

Waiting for the User
The following line of the program displays the prompt and, the statement saying “Press the enter key to exit”, and then waits for the user to take action −

#!/usr/bin/python3

input("\n\nPress the enter key to exit.")
Here, "\n\n" is used to create two new lines before displaying the actual line. Once the user presses the key, the program ends. This is a nice trick to keep a console window open until the user is done with an application.

Multiple Statements on a Single Line
The semicolon ( ; ) allows multiple statements on a single line given that no statement starts a new code block. Here is a sample snip using the semicolon −

import sys; x = 'foo'; sys.stdout.write(x + '\n')
Multiple Statement Groups as Suites
Groups of individual statements, which make a single code block are called suites in Python. Compound or complex statements, such as if, while, def, and class require a header line and a suite.

Header lines begin the statement (with the keyword) and terminate with a colon ( : ) and are followed by one or more lines which make up the suite. For example −

if expression : 
   suite
elif expression : 
   suite 
else : 
   suite
Command Line Arguments
Many programs can be run to provide you with some basic information about how they should be run. Python enables you to do this with -h −

$ python -h
usage: python [option] ... [-c cmd | -m mod | file | -] [arg] ...
Options and arguments (and corresponding environment variables):
-c cmd : program passed in as string (terminates option list)
-d     : debug output from parser (also PYTHONDEBUG=x)
-E     : ignore environment variables (such as PYTHONPATH)
-h     : print this help message and exit

[ etc. ]
You can also program your script in such a way that it should accept various options. Command Line Arguments is an advanced topic. Let us understand it.
