# C-shanties Programming Language Documentation

## Introduction

C-shanties be a pirate-themed programming language that brings the spirit of the high seas to the world of code. With its unique lingo and syntax, it allows ye to write programs fit for a buccaneer. This documentation be yer guide to understanding and using C-shanties to craft yer own pirate code adventures.

## Grammar

### Variables

To declare a variable, use the `chest` keyword followed by the data type and the variable name:

```
chest <type> <name>;
```

#### Data Types

C-shanties supports the following data types:

* `doubloon`: Represents numeric integer values.
* `piecesOfEight` : Represents numeric floating point values.
* `scroll`: Represents text or strings.
* `buccaneer`: Represents characters.
* `rum`: represents boolean values.
    * `aye`: Represents the boolean value true.
    * `nay`: Represents the boolean value false.
* arrays are represented by appending `[]` to the data type.

Examples:

```
chest doubloon x =  10;
chest scroll message ="Ahoy, matey!";
chest rum treasureFound = aye;
chest buccaneer initial = 'A';
```

### Assigning Values

To assign a value to a variable, use the assignment operator `=`:

```
<name> = <value>;
```

Examples:

```
x = 10;
message = "Ahoy, matey!";
treasureFound = aye;
```

### Conditionals

C-shanties provides conditional statements to control the flow of yer code.

#### If Statement

To perform an action if a condition be true, use the `avast` keyword:

```
avast (<condition>) {
    // Code block to be executed if condition be true
}
```

Example:

```
avast (treasureFound == aye) {
    ahoy("Avast, ye found the treasure!");
}
```

#### If-Else Statement

To perform different actions based on a condition, use the `avast` for if and `belay` for else keyword:

```
avast (<condition>) {
    // Code block to be executed if condition be true
} belay {
    // Code block to be executed if condition be false
}
```

Example:

```
avast (treasureFound == aye) {
    ahoy("Avast, ye found the treasure!");
} belay {
    ahoy("No treasure in sight, matey!");
}
```

### Loops

C-shanties provides looping mechanisms to repeat code execution.

#### While Loop

To repeat a code block while a condition be true, use the `while` keyword:

```
while (<condition>) {
    // Code block to be executed while condition be true
}
```

Example:

```
doubloon count = 0d;
while (count < 10d) {
    ahoy("Count: ", count);
    count = count + 1d;
}
```

#### For Loop

To iterate over a range of values, use the `sail` keyword followed by initialization, condition, and increment:

```
sail (<initialization>; <condition>; <increment>) {
    // Code block to be executed repeatedly until condition be false
}
```

Example:

```
sail (chest doubloon i = 0d; i < 5d; i = i + 1d) {
    ahoy("Yo ho! Iteration ", i);
}
```

### Functions

C-shanties allows ye to define and call yer own functions.

#### Function Declaration

To declare a function, use the `parley` keyword followed by the return type, function name, and parameters:

```
parley <return_type> <function_name>(<parameters>) {


    // Code block for the function
}
```

Example:

```
parley doubloon calculateSum(doubloon a, doubloon b) {
    chest doubloon sum = a + b;
    return sum;
}
```

#### Function Call

To call a function, use the function name followed by parentheses and arguments:

```
<function_name>(<arguments>);
```

Example:

```
doubloon result = calculateSum(5d, 7d);
ahoy("Sum: ", result);
```

### Input and Output

C-shanties allows ye to read input and display output.

#### Input

To read input from the user, use the `ayeCaptain` keyword followed by the variable name:

```
ayeCaptain <variable>;
```

Example:

```
ayeCaptain doubloon x;
```

#### Output

To display output, use the `ahoy` keyword followed by the value or variable to be printed:

```
ahoy(<value>);
```

Example:

```
ahoy("Ahoy, matey!");
ahoy(x);
```

### Comments

C-shanties supports both single-line and multi-line comments.

#### Single-line Comment

To add a single-line comment, use the "shiver me timbers!" expression followed by the comment text:

```
shiver me timbers! <comment_text>
```

Example:

```
shiver me timbers! This be a comment, matey!
```

#### Multi-line Comment

To add a multi-line comment, use the "shiver me timbers!" expression followed by each line of the comment and end it with a blank line.:

```
shiver me timbers!
<comment_line_1>
<comment_line_2>
...

```

Example:

```
shiver me timbers!
This be the first line of me comment.
And this be the second line.

```

## Examples

Here be some examples to get ye started on yer pirate coding journey:

1. Hello, World! in C-shanties:

```
ahoy("Ahoy, world!");
```

2. Count from 1 to 10:

```
sail (chest doubloon i = 1d; i <= 10d; i = i + 1d) {
    ahoy(i);
}
```

3. Calculate the factorial of a number:

```
parley doubloon factorial(doubloon n) {
    avast (n <= 0d) {
        return 1d;
    } else {
        return n * factorial(n - 1d);
    }
}

chest doubloon number = 5d;
doubloon result = factorial(number);
ahoy("Factorial of ", number, " is ", result);
```



---
---

## Class Declaration

To declare a ship (class) in C-shanties, ye can use the keyword "ship" followed by the ship name:

```
ship <ship_name> {
    // Class members and methods go here
}
```

## Constructor (Beginsail)

To define the constructor (the function called when a new ship object be created), ye can use the keyword "beginsail" followed by any parameters:

```
beginsail(<parameters>) {
    // Constructor code goes here
}
```

Example:
```
ship Pirate {
    beginsail() {
        ahoy("A new pirate has set sail!");
    }
}
```

## Class Members

Inside a ship declaration, ye can define class members, such as variables and functions. These members can be accessed within the class methods.

### Variables

To define class variables, use the "chest" keyword within the ship declaration:

```
chest <type> <name>;
```

Example:
```
ship Pirate {
    chest doubloon treasures;
    chest scroll name;
}
```

### Methods

To define class methods, use the traditional function declaration syntax within the ship declaration:

```
<method_visibility> <return_type> <method_name>(<parameters>) {
    // Method code goes here
}
```

Example:
```
ship Pirate {
    chest doubloon treasures;

    parley void celebrate() {
        ahoy("Arr, we be celebratin'!");
    }

    parley doubloon countTreasures() {
        return treasures;
    }
}
```

## Creating Objects

To create an object (instance) of a ship (class) in C-shanties, ye can use the ship name followed by parentheses:

```
ship_name <object_name>;
```

Example:
```
Pirate jack;
```

## Accessing Members

To access ship members (variables and methods), ye can use the object name followed by a dot (.) and the member name:

```
<object_name>.<member_name>
```

Example:
```
jack.treasures = 5;
ahoy(jack.countTreasures());
```

## Conclusion

With this documentation, ye be ready to set sail on yer ship (class) adventures in C-shanties! Explore the vast sea of object-oriented programming, define classes, create objects, and access members like a true pirate of the code world. Yo ho, me hearties, happy object-oriented coding!




---
# future plans

* Static Members
* Final Members
* Inheritance
---
