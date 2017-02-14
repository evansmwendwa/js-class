## JavaScript Syntax

JavaScript `syntax` is the set of rules, how JavaScript programs are constructed.

## JavaScript Programs

A **computer program** is a list of "instructions" to be "executed" by the computer.

In a programming language, these program instructions are called **statements**.

JavaScript is a programming language.

JavaScript statements are separated by **semicolons**:

### Example

``` javascript
var x, y, z;
x = 5;
y = 6;
z = x + y;
```
## JavaScript Statements

JavaScript statements are composed of:

Values, Operators, Expressions, Keywords, and Comments.

## JavaScript Values

The JavaScript syntax defines two types of values: Fixed values and variable values.

Fixed values are called literals. Variable values are called variables.

## JavaScript Literals
The most important rules for writing fixed values are:

Numbers are written with or without decimals:
``` javascript
10.5
1000
0.562
3.1415
-56
```

Strings are text, written within double or single quotes:
``` javascript
"John Doe"
'Jane Doe'
```
## JavaScript Variables

In a programming language, variables are used to store data values.

JavaScript uses the var keyword to declare variables.

An equal sign is used to assign values to variables.

In this example, x is defined as a variable. Then, x is assigned (given) the value 6:

``` javascript
var x;
x = 6;
```

## JavaScript Operators
JavaScript uses arithmetic operators ( + - *  / ) to compute values:

``` javascript
(5 + 6) * 10
```
JavaScript uses an assignment operator ( = ) to assign values to variables:
``` javascript
var x, y;
x = 5;
y = 6;
```

## JavaScript Expressions
An expression is a combination of values, variables, and operators, which computes to a value.

The computation is called an evaluation.

For example, 5 * 10 evaluates to 50:
``` javascript
5 * 10
```

Expressions can also contain variable values:
``` javascript
var x;
x = 5;
x * 10;
```
The values can be of various types, such as numbers and strings.

For example, "John" + " " + "Doe", evaluates to "John Doe":

``` javascript
"John" + " " + "Doe"
```

## JavaScript Keywords

JavaScript **keywords** are used to identify actions to be performed.

The **var** keyword tells the browser to create variables:

``` javascript
var x, y;
x = 5 + 6;
y = x * 10;
```

## JavaScript Comments

Not all JavaScript statements are "executed".

Code after double slashes // or between /* and */ is treated as a comment.

Comments are ignored, and will not be executed:

Comments can be used to describe what you code does.

``` javascript
var x = 5;   // I will be executed

// var x = 6;   I will NOT be executed
```

## JavaScript Identifiers

Identifiers are names.

In JavaScript, identifiers are used to name variables (and keywords, and functions, and labels).

The rules for legal names are much the same in most programming languages.

In JavaScript, the first character must be a letter, an underscore (_), or a dollar sign ($).

Subsequent characters may be letters, digits, underscores, or dollar signs.

> Numbers are not allowed as the first character.
This way JavaScript can easily distinguish identifiers from numbers.

## JavaScript is Case Sensitive

All JavaScript identifiers are **case sensitive**. 

The variables **lastName** and **lastname**, are two different variables.

``` javascript
var lastname, lastName;
lastName = "Doe";
lastname = "Peterson";
```
> JavaScript does not interpret `VAR` or `Var` as the keyword `var`.

## JavaScript and Camel Case
Historically, programmers have used three ways of joining multiple words into one variable name:

**Hyphens:**
``` javascript
first-name, last-name, master-card, inter-city.
```
> Hyphens are not allowed in JavaScript. It is reserved for subtractions.

**Underscore:**
``` javascript
first_name, last_name, master_card, inter_city.
```

**Camel Case:**
``` javascript
FirstName, LastName, MasterCard, InterCity.
```
> JavaScript programmers tend to use camel case that starts with a lowercase letter:
``` javascript
firstName, lastName, masterCard, interCity.
```

> **< Previous Lesson** ([Lesson 2 - Scripting](https://github.com/evansmwendwa/js-class/blob/master/02-Scripting.md)) **| Next Lesson >** ([Lesson 4 - Statements](https://github.com/evansmwendwa/js-class/blob/master/04-Statements.md))
