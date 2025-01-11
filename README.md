# pcep-notes
Notes for my PCEP cert. Do I even need this?

## to-do list
* go through videos
* flashcards if there's anything I don't already know
* take PCEP test

## primary source
https://www.udemy.com/course/python-pcep

## PCEP sections and mapping
1. Fundamentals ➡️ Module 1 & 2
2. Control Flow ➡️ Module 3
3. Data Collections ➡️ Module 4
4. Functions and Exceptions ➡️ Module 5

## module 1: basic concepts
* covers ```print```
    * printing apostophes using double quotes around singles
    * using escape character
    * all prints have a newline at the end
    * ```\n``` is newline
* variables
    * must start with a letter or underscore, no numbers
    * case sensitive
    * protected names (from, global, etc.)
* data types
    * strings
    * int (whole numbers)
    * floats (decimals)
    * boolean (```True``` or ```False```, case sensitive)
    * COMMENT: more types to come later...
* comments
    * uses hash, turns rest of the line into comment
* numerical representations
    * as of 3.6, you can use underscores in numbers to improve readability
        * ```12_000_300``` = ```120003000```
    * scientific notation
        * 3e4 or 3E4 = 3 * 10000 = 30000
        * 3e-4 = 3 * .0001 = .0003
    * octal numbers
        * ```0o123```
    * hex
        * ```0x123```
* operators
    * addition +
    * subtraction -
    * multiplication *
    * division
        * / standard, produces float, regardless of dividing ints
        * // integer division, nearest whole number, rounded down
        * % modulo, returns just remainder
        * never divide by zero (ZeroDivisionError)
    * powers/exponents **
* extra: how does modulo work?
* assigning values
    * can multiple strings, never knew
* input() function
    * always returns a string type
* technical theory
    * translate from source to machine code
    * compilation or interpretation
        * comp = executable file (compile once)
        * inter = runs on the fly (this is Python)
            * "scripting language"
    * py executes top to bottom
        * lexis, syntax, semantics
            * lexis = reserved terms in Python
            * syntax
            * semantics
(Passed post module test, 14/15.)

## module 2: data types, evals, basic i/o
* typecasting
    * changing variable types
* more re: operators
    * binary operators (require two values), ```+ - * / // %```
    * unary operators for making positive/negative
* order of operations
    * PEMDAS
* floating point accuracy
    * floats are more-or-less right, but not 100%
    * precision is limited
* exponents and order of operations:
    * without parenthesis, it starts from the right and goes to the left
    * thus ```2 ** 3 ** 4``` is the same as ```2 ** (3 ** 4)```
* more print and strings
    * covering ```len()```
    * kwargs (keyword args)
        * end can be used to redefine an endline character
        * sep argument is used to redefine spacing between strings in a print
* bit operators
    * probably shouldn't be in PCEP; but it is
    * operators: ```& | ~ ^ << >>```
        * & and
        * | or
        * ^ xor
        * ~ not
        * << >> shift bit
        * << 1 = double
        * << 2 = four
        * >> 1 = half
        * >> 2 = quarter
    * how to convert binary to decimal

## module 3: control flow, conditionals, loops
* if statements
    if else elif (else if)
    
* logical operators and conditions

* joining multiple conditions
* nested if statements
* while loops
* for loops
* break and continue
* other loop features


## module 4: data collections

## module 5: functions and exceptions

