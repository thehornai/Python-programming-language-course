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

Mac OS
Download Mac OS installers from this URL − https://www.python.org/downloads/mac-osx/

Mac OS X 64-bit/32-bit installer − python-3.5.1-macosx10.6.pkg
Mac OS X 32-bit i386/PPC installer − python-3.5.1-macosx10.5.pkg
Double click this package file and follow the wizard instructions to install.

The most up-to-date and current source code, binaries, documentation, news, etc., is available on the official website of Python −

Python Official Website − https://www.python.org/

You can download Python documentation from the following site. The documentation is available in HTML, PDF and PostScript formats.

Python Documentation Website − www.python.org/doc/

Setting up PATH
Programs and other executable files can be in many directories. Hence, the operating systems provide a search path that lists the directories that it searches for executables.

The important features are −

The path is stored in an environment variable, which is a named string maintained by the operating system. This variable contains information available to the command shell and other programs.

The path variable is named as PATH in Unix or Path in Windows (Unix is case-sensitive; Windows is not).

In Mac OS, the installer handles the path details. To invoke the Python interpreter from any particular directory, you must add the Python directory to your path.

Setting Path at Unix/Linux
To add the Python directory to the path for a particular session in Unix −

In the csh shell − type setenv PATH "$PATH:/usr/local/bin/python3" and press Enter.

In the bash shell (Linux) − type export PYTHONPATH=/usr/local/bin/python3.4 and press Enter.

In the sh or ksh shell − type PATH = "$PATH:/usr/local/bin/python3" and press Enter.

Note − /usr/local/bin/python3 is the path of the Python directory.

Setting Path at Windows
To add the Python directory to the path for a particular session in Windows −

At the command prompt − type path %path%;C:\Python and press Enter.

Note − C:\Python is the path of the Python directory

Python Environment Variables
Here are important environment variables, which are recognized by Python −

Sr.No.	Variable & Description
1	
PYTHONPATH

It has a role similar to PATH. This variable tells the Python interpreter where to locate the module files imported into a program. It should include the Python source library directory and the directories containing Python source code. PYTHONPATH is sometimes preset by the Python installer.

2	
PYTHONSTARTUP

It contains the path of an initialization file containing Python source code. It is executed every time you start the interpreter. It is named as .pythonrc.py in Unix and it contains commands that load utilities or modify PYTHONPATH.

3	
PYTHONCASEOK

It is used in Windows to instruct Python to find the first case-insensitive match in an import statement. Set this variable to any value to activate it.

4	
PYTHONHOME

It is an alternative module search path. It is usually embedded in the PYTHONSTARTUP or PYTHONPATH directories to make switching module libraries easy.

Running Python
There are three different ways to start Python −

Interactive Interpreter
You can start Python from Unix, DOS, or any other system that provides you a command-line interpreter or shell window.

Enter python the command line.

Start coding right away in the interactive interpreter.

$python             # Unix/Linux
or
python%             # Unix/Linux
or
C:>python           # Windows/DOS
Here is the list of all the available command line options −

Sr.No.	Option & Description
1	
-d

provide debug output

2	
-O

generate optimized bytecode (resulting in .pyo files)

3	
-S

do not run import site to look for Python paths on startup

4	
-v

verbose output (detailed trace on import statements)

5	
-X

disable class-based built-in exceptions (just use strings); obsolete starting with version 1.6

6	
-c cmd

run Python script sent in as cmd string

7	
file

run Python script from given file

Script from the Command-line
A Python script can be executed at the command line by invoking the interpreter on your application, as shown in the following example.

$python  script.py          # Unix/Linux
or
python% script.py           # Unix/Linux
or 
C:>python script.py         # Windows/DOS
Note − Be sure the file permission mode allows execution.

Integrated Development Environment
You can run Python from a Graphical User Interface (GUI) environment as well, if you have a GUI application on your system that supports Python.

Unix − IDLE is the very first Unix IDE for Python.

Windows − PythonWin is the first Windows interface for Python and is an IDE with a GUI.

Macintosh − The Macintosh version of Python along with the IDLE IDE is available from the main website, downloadable as either MacBinary or BinHex'd files.

If you are not able to set up the environment properly, then you can take the help of your system admin. Make sure the Python environment is properly set up and working perfectly fine.

Note − All the examples given in subsequent chapters are executed with Python 3.4.1 version available on Windows 7 and Ubuntu Linux.

We have already set up Python Programming environment online, so that you can execute all the available examples online while you are learning theory. Feel free to modify any example and execute it online.
