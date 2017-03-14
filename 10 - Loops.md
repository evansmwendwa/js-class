## JavaScript Loops

Loops can execute a block of code a number of times.

Loops are handy, if you want to run the same code over and over again, each time with a different value.

Often this is the case when working with arrays:

**Instead of writing**

```
text += cars[0] + "<br>"; 
text += cars[1] + "<br>"; 
text += cars[2] + "<br>"; 
text += cars[3] + "<br>"; 
text += cars[4] + "<br>"; 
text += cars[5] + "<br>";
```

**You can use a loop to simplify your code to just a few lines**

``` javascript
for (i = 0; i < cars.length; i++) { 
    text += cars[i] + "<br>";
}
```

## Different Kinds of Loops

JavaScript supports different kinds of loops:

* **for** - loops through a block of code a number of times
* **for/in** - loops through the properties of an object
* **while** - loops through a block of code while a specified condition is true
* **do/while** - also loops through a block of code while a specified condition is true

## The For Loop

### Syntax

```
for (statement 1; statement 2; statement 3) {
    code block to be executed
}
```

`Statement 1` is executed before the loop (the code block) starts.

`Statement 2` defines the condition for running the loop (the code block).

`Statement 3` is executed each time after the loop (the code block) has been executed.

### Example

``` javascript
var text = '';

for (i = 0; i < 5; i++) {
    text += "The number is " + i + "<br>";
}

document.write(text);
```

From the example above, you can read:

`Statement 1` sets a variable before the loop starts (var i = 0).

`Statement 2` defines the condition for the loop to run (i must be less than 5).

`Statement 3` increases a value (i++) each time the code block in the loop has been executed.

## The For/In Loop

The JavaScript for/in statement loops through the properties of an object:

### Example

``` javascript
var person = {fname:"John", lname:"Doe", age:25}; 

var text = "";
var x;
for (x in person) {
    text += person[x];
}
```

## The While Loop

The while loop loops through a block of code as long as a specified condition is true.

### Syntax

```
while (condition) {
    code block to be executed
}
```

### Example

In the following example, the code in the loop will run, over and over again, as long as a variable (i) is less than 10:

``` javascript
while (i < 10) {
    text += "The number is " + i;
    i++;
}
```

## The Do/While Loop

The do/while loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

### Syntax

```
do {
    code block to be executed
}
while (condition);
```

### Example

The example below uses a do/while loop. The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested:

``` javascript
do {
    text += "The number is " + i;
    i++;
}
while (i < 10);
```
**NB:** Do not forget to increase the variable used in the condition, otherwise the loop will never end!

## JavaScript Break and Continue

The break statement "jumps out" of a loop.

The continue statement "jumps over" one iteration in the loop.

### The Break Statement

You have already seen the break statement in the earlier chapters. We used a `break` to jump out ofa `switch()` statement.

The break statement can also be used to jump out of a loop.  

The break statement breaks the loop and continues executing the code after the loop (if any):

``` javascript 

for (i = 0; i < 10; i++) {
    if (i === 3) { break; }
    text += "The number is " + i + "<br>";
}

```

### The Continue Statement

The continue statement breaks one iteration (in the loop), if a specified condition occurs, and continues with the next iteration in the loop.

``` javascript
for (i = 0; i < 10; i++) {
    if (i === 3) { continue; }
    text += "The number is " + i + "<br>";
}
```
