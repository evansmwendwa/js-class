## JavaScript Statements
In HTML, JavaScript statements are "instructions" to be "executed" by the web browser.

This statement tells the browser to write "Hello Dolly." inside an HTML element with id="demo":

``` javascript
document.getElementById("demo").innerHTML = "Hello Dolly.";
```

## JavaScript Programs

Most JavaScript programs contain many JavaScript statements.

The statements are executed, one by one, in the same order as they are written.

In this example x, y, and z are given values, and finally z is displayed:

``` javascript
var x, y, z;
x = 5;
y = 6;
z = x + y;
document.getElementById("demo").innerHTML = z;
```

> JavaScript programs (and JavaScript statements) are often called JavaScript code.

## Semicolons ;

Semicolons separate JavaScript statements.

Add a semicolon at the end of each executable statement:

``` javascript
var a, b, c;
a = 5;
b = 6;
c = a + b;
```

> When separated by semicolons, multiple statements on one line are allowed:

``` javascript
a = 5; b = 6; c = a + b;
```

> On the web, you might see examples without semicolons. 
Ending statements with semicolon is not required, but highly recommended.

## JavaScript White Space

JavaScript ignores multiple spaces. You can add white space to your script to make it more readable.

The following lines are equivalent:

``` javascript
var person = "Hege";
var person="Hege";
```

> A good practice is to put spaces around operators ( = + - * / ):

```
var x = y + z;
```

## JavaScript Line Length and Line Breaks

For best readability, programmers often like to avoid code lines longer than 80 characters.

If a JavaScript statement does not fit on one line, the best place to break it, is after an operator:

``` javascript
document.getElementById("demo").innerHTML =
"Hello Dolly.";
```

## JavaScript Code Blocks

JavaScript statements can be grouped together in code blocks, inside curly `brackets {...}`.

The purpose of code blocks is to define statements to be executed together.

One place you will find statements grouped together in blocks, is in JavaScript functions:

``` javascript
function myFunction() {
    document.getElementById("demo1").innerHTML = "Hello Dolly.";
    document.getElementById("demo2").innerHTML = "How are you?";
}
```

