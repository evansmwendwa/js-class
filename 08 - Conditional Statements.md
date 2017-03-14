## JavaScript `if` Statement

The "If Statement" is a way to make decisions based on a variable or some other type of data. For example, you might have a variable that stores the date. With this tiny bit of information, you can easily program a small script to print out, "Today is my Birthday!" whenever the day and month were equal to your birthday.

There are two major parts to an If Statement: the conditional statement and the code to be executed.

The conditional statement is a statement that will evaluate to be either True or False. The most common type of conditional statement used checks to see if something equals a value. An example would be checking if a date equals your birthday.

Below is a segment of JavaScript code that will be executed only if the If Statement's conditional statement is true. In this simple If Statement example, we print out a message if the variable we are checking is equal to 7.

``` javascript
var myNum = 7;

if(myNum == 7){
  document.write("Lucky 7!");
}
```

## JavaScript `if` statement: `else`

The Else clause is executed when the conditional statement is False. Let's take our example from above, add an Else clause, and change the value of myNum so that our conditional statement is False.

``` javascript
var myNum = 10;

if(myNum == 7){
  document.write("Lucky 7!");
}else{	
  document.write("You're not very lucky today...");	
}
```

## JavaScript `else if` statement

The Else If statement is an extension to the If Statement that allows you to create as many checks (conditional statements) as you want in one big block of If Statement code.

Imagine that you want to have a small "student" script that will print out a customized message depending who is accessing the webpage. If you have more than two custom messages, you could use the Else If extension to solve this programming problem.

``` javascript
var visitor = "principal";

if(visitor == "teacher"){
  document.write("My dog ate my homework...");
} else if(visitor == "principal"){
  document.write("The tyrant is in!");
} else {
  document.write("How do you do?");
}
```
There are two important things to note about the `Else If` extension:

* You must have a normal If Statement before you can use the Else If statement. This is because the Else If statement is an addon to the If Statement.
* You can have multiple Else If add-ons. In our example, we only used one Else If extension, but you can add as many as you require.

## JavaScript Switch Statement

The switch statement is used to perform different actions based on different conditions.
Use the switch statement to select one of many blocks of code to be executed.

## Syntax

``` javascript
switch(expression) {
    case n:
        code block
        break;
    case n:
        code block
        break;
    default:
        code block
}
```
**This is how it works:**

* The switch expression is evaluated once.
* The value of the expression is compared with the values of each case.
* If there is a match, the associated block of code is executed.

## Example

The following example prints the current day of the week in your browser.
The switch statement gets the current day (number) from the date object then performs conditional checks to create the textual representation of the day.

**NB:** The starting day of the week (0) is sunday.

**NB:** If you forget adding a break in any `case` statement the next statement will also be executed.

``` javascript
var day;

switch (new Date().getDay()) {
    case 0:
        day = "Sunday";
        break;
    case 1:
        day = "Monday";
        break;
    case 2:
        day = "Tuesday";
        break;
    case 3:
        day = "Wednesday";
        break;
    case 4:
        day = "Thursday";
        break;
    case 5:
        day = "Friday";
        break;
    case 6:
        day = "Saturday";
}

document.write(day);
```
