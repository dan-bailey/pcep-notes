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
    * < > <= >= == !=
* joining multiple conditions
    * ```and or not```
    * priority: not, and, or
* nested if statements
    * easy easy (no notes)
* while loops
    * easy easy (no notes)
    * used for unknown number of steps
* for loops
    * used for a known number of steps
    * no conditionals
    * easy easy (no notes)
* break and continue
    * break is for exiting a loop
    * great for getting out of a shitty while loop
    * continue is good for skipping back to the conditional
* other loop features
    * pass requires instruction in a loop; it can be used as a placeholder so code doesn't throw errors (works in loops and if/else logic)
    * nested loops, easy
    * loops with else (seldom used/rare)
        * else always get executed after a loop finishes
    
## module 4: data collections
* intro to lists
    * they're arrays, duh
    * indexing is the same
    * i am annoyed by the terminology change
    * slicing
        * ```top_cities[0:2]```
        * returns the first two items in the list, first val is starting point, second val is the point where you don't share, i.e.: end here, but don't display.
        * ```top_cities[2:]``` means start at element 2 (the third element) and continue through the remainder of the list
        * ```top_cities[:3]``` start at the beginning and go through until index 3, but don't show index 3
* deleting list elements
    * ```del``` deletes -- use as: ```del top_cities[2]```
    * elements nuked this way have their space filled-in as all following items in the list are shifted left
    * can use slicing to remove in a similar methodology
    * ```del top_cities[3:]``` removes everything from index 3 onward
* adding lists elements
    * use ```.append()``` method to add to the end of the list
    * use ```.insert(x, y)``` method to insert value y at location x in the list
* iterating lists
    * ```for item in list_name:``` you lose index value here, though
    * ```for idx in range(len(top_cities):``` then index each item by idx like ```top_cities[idx]```
* changing element positions
    * doesn't require a temp in python
    * just do ```var_1, var_2 = var_2, var_1```
    * applies to lists with an index, just the same way
    * ```.sort()``` method destroys original
    * as a temporary function, you can use ```sorted(list_name)``` to output results similar to .sort() without impacting the original list
* checking element presence
    * ```if val in list_name:```
    * ```if val not it list_name:```
* copying lists
    * if you have list_1 and do: ```list_2 = list_1``` you're making a copy of a reference to the list, so changing element[0] changes it in both
    * if you use slicing you get two unique lists where memory is concerned -- do ```list_2 = list_1[:]
    * also use slicing to copy a fragment of the original into the new list
* list comprehension
    * ```numbers = [i for i in range(1,101)]```
    * ```numbers = [i for i in range(1,100) if i % 3 != 0]```
* nested lists
    * ```test = [['A1', 'A2', 'A3'], [['B1', 'B2', 'B3']]```
    * ```test[0] == ['A1', 'A2', 'A3']```
    * ```test[0][2] == 'A3'```
* adding and multiplying lists
* further string features
* intro to tuples
    * tuple operations
    * tuples in lists, lists in tuples
* intro to dictionaries
    * dictionary operations

## module 5: functions and exceptions

