# Patroclus Interpreter

Patroclus is an interpreter of a small programming language, written in Python 3. Its basic code was taken from davidcallanan's project and later developed by Klaus Bluseng.

<br>
<p align="center">
  <img src="https://github.com/FerdosiaEngine/VATA/blob/main/1.5.png?raw=true">
</p>

## Current version and project content

The current version of the interpreter is 1.1. The project folder consists of several small files, needed to run a code sequence specific to this language. For optimal operation and return of the correct result, these tabs cannot be modified.

## Way of usage

The dependence of the current program is represented by the existence of the Python 3 programming language.

You also need to add the Python path to the Windows Path variable (which will be searched for executables when you type a command at the command prompt), if it doesn't already exist.

After downloading the interpreter files we are almost ready to run the code. All we have to do is open the command prompt, where we will enter the whole path to the folder where the execution files are, in the form:

```
cd C:\...\Patroclus
```

After setting the path, the command to execute the interpreter code will be used, which is as follows:

```
python shell.py
```

To execute a unique sequence of code, it can be written directly in the command prompt, which will display the result. However, it is recommended to write the code in an external file. The following command runs an external file called EXP.vata, located in the same path as the program:

```
RUN("EXP.vata")
```

To display the code result, the file must exist and be written according to the grammar rules recognized by the interpreter.

## Quick start in the grammatical structure of the interpreter

The order of mathematical operations is respected by the use of parentheses. Numbers are classified as integers and decimals. Different mathematical operators are: "+", "-", "*", "/", "^", "OR", "AND", ">", "<", ">=", "<=", "=", "!=".

The presence of a comma at the end of a line of code is not required. The "PRINT()" function prints the specified message to the screen. The message can be a string or a number.

```
PRINT("Hello world!")
PRINT(1 + 8 - 6)
PRINT(7 ^ 2 / 2)
PRINT(8 / (9 - 3))
PRINT(5.78 + 9.23)
PRINT(2 > 7)
PRINT(4 <= 8)
PRINT(19 != 22)
```

A variable is defined by using the "VAR" specific keyword, followed by the name of the variable. Data entry from the user is performed with the "INPUT()" function. Comments are made on a single line, which must start with #.

```
# This is a comment.

VAR D = "QWERTY" + "ASDF"
VAR B = 10
VAR A = 8
VAR C = A + B
PRINT(C)

PRINT("Enter input: ")
VAR X = INPUT()
PRINT("Your input: " + X)
```

Below is a list of predefined functions.

```
NULL, FALSE, TRUE, MATH_PI, PRINT, PRINT_RET, INPUT, INPUT_INT, CLEAR, CLS, IS_NUM, IS_STR, IS_LIST, IS_FUN, APPEND, POP, EXTEND, LEN, RUN.
```

The concept of "LISTS" is similar to that of the python language. The structure of the "IF, ELIF, ELSE, WHILE, FOR" functions IS DIFFERENT, as follows:

```
FOR E = 1 TO 9 THEN E * 7
VAR B = 10; VAR A = 8; IF A > B THEN "A is greater" ELSE "B is greater"
VAR Q = 1; WHILE Q < 10000 THEN VAR Q = Q + 1
```

For more details on the structure, see the grammer.txt file.

## Ferdosia Engine

GitHub: https://github.com/FerdosiaEngine
