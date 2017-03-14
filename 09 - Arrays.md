## JavaScript Array

An array is a variable that can store many variables within it. Many programmers have seen arrays in other languages, and they aren't that different in JavaScript.

* The array is a special type of variable.
* Values are stored into an array by using the array name and	by stating the location in the array you wish to store the value in brackets. Example: myArray[2] = "Hello World";
* Values in an array are accessed by the array name and location of the value. Example: myArray[2];
* JavaScript has built-in functions for arrays that allow us to do things with them like, iterating, searching, adding, delete and many more

## Creating a JavaScript Array

Creating an array is slightly different from creating a normal variable. Because JavaScript has variables and properties associated with arrays, you have to use a special function to create a new array. This example shows how you would create a simple array, store values to it, and access these values.

### Syntax

``` javascript
var array_name = [item1, item2, ...];    
```

### Examples

``` javascript
var sports = ["Football", "Baseball", "Cricket"];
```

You can also assign values to an array by specifying the array index
``` javascript
var myArray = new Array();

sports[0] = "Football";
sports[1] = "Baseball";
sports[2] = "Cricket";

```

Spaces and line breaks are not important. A declaration can span multiple lines:

``` javascript
var sports = [
    "Football",
    "Baseball",
    "Cricket"
];
```

Using the JavaScript Keyword new

``` javascript
var sports = new Array("Football", "Baseball", "Cricket");
```

## Accessing Elements of an Array
You refer to an array element by referring to the index number.

This statement accesses the value of the first element in `sports` array:
``` javascript
var sports = sports[0];
```

## Accessing the Full Array

``` javascript
var sports = ["Football", "Baseball", "Cricket"];
document.getElementById("demo").innerHTML = sports;
``` 

## Array Properties and Methods

``` javascript
var x = sports.length;
var y = sports.sort();

console.log(x,y);
```

## The length Property
The length property of an array returns the length of an array (the number of array elements).

``` javascript
var sports = ["Football", "Baseball", "Cricket"];
var count = sports.length;  // will return the total number of items in the array i.e 3
```

## Adding Array Elements
The easiest way to add a new element to an array is using the push method:

``` javascript
var sports = ["Football", "Baseball", "Cricket"];
sports.push("Volleyball");
```

**New element can also be added to an array using the length property:**

``` javascript
var sports = ["Football", "Baseball", "Cricket"];
sports[sports.length] = "Hockey";
```

## The Difference Between Arrays and Objects
In JavaScript, arrays use numbered indexes.  

In JavaScript, objects use named indexes.

```
Arrays are a special kind of objects, with numbered indexes.
```

## When to Use Arrays. When to use Objects.

* JavaScript does not support associative arrays.
* You should use objects when you want the element names to be strings (text).
* You should use arrays when you want the element names to be numbers.

## Avoid new Array()
There is no need to use the JavaScript's built-in array constructor new Array().

**Use [] instead.**

These two different statements both create a new empty array named points:

``` javascript
var points = new Array();         // Long
var points = [];                  // Short 
```

The `new` keyword only complicates the code. It can also produce some unexpected results:

``` javascript
var points = new Array(40, 100); // Creates an array with two elements (40 and 100)
```

What if I remove one of the elements?

``` javascript
var points = new Array(40); // Creates an array with 40 undefined elements !!!!!
```
