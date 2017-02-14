## Writing your first JavaScript Application

**Where to write your JavaScript Code:**
JavaScript Code can be written in any text editor that supports plain text encoding.
**E.g:** Notepad, Sublime Text, Atom, Brackets

JavaScript Code can also be written using Code Editors that are available in the web.
**E.g:** [JSfiddle](https://jsfiddle.net/), [Plunker](https://plnkr.co/), [CodePen](https://codepen.io/)

> JavaScript can not be written in word processors like Microsoft Word and Wordpad because they don't support plain text formats.

In HTML, JavaScript code must be inserted between `<script>` and `<script>` tags

**Example:**
``` javascript
<script>
alert('This is my first JS application');
</script>
```

**JavaScript in `<head>` or `<body>`**
You can place any number of scripts in an HTML document.
Scripts can be placed in the `<body>`, or in the `<head>` section of an HTML page, or in both.

**EXAMPLE**

``` javascript
<!DOCTYPE html>
<html>
<head>
<script>
function greeting() {
    alert('Hello People');
}
</script>
</head>

<body>

<h1>JavaScript Application</h1>
<button type="button" onclick="greeting()">Try it</button>

</body>
</html>
```

**External JS Files**
JavaScript can be written in external files that can be embedded in your HTML document using the` <script>` tag.
In order to embed external JS file you must use the src attribute on the script tag and provide either the relative path or the absolute path to the external JS file.
It's common behaviour to name your external JS files with the `.js` file extension.

**Note:** you can place external scripts in either the `<head>` or the `<body>` as you like.

**Example**
``` javascript
<script src="application.js"></script>
<script src="https://google.com/cdn/jsquery.min.js"><script>
```

``` javascript
// file named application.js in the same location as the html document
// Functions in this file can be called if the file us embedded
// in your html document

function myFunction() {
   alert('Wassup guys!');
}
```

####External JavaScript Advantages
Placing scripts in external files has some advantages:
* It separates HTML and JavaScript code
* It makes HTML and JavaScript easier to read and maintain
* External JS files can be cached by the browser hence speeding up page loads

###Debugging JavaScript
When writing your applications you will need a way to debug and figure our when errors occur. Most browsers provide developer tools that allow you to test different scenarios and execute code that only you the developer can see.

The best tool for this is the browser console which display errors and console logs.

You can open the console by pressing `Ctrl` + `Shift` + `I` (Simultaneously) in your firefox or chrome browser

To output code to your browser console pass your variable or output to the `console.log()` method.
**Example**

``` javascript
<script>
console.log('JavaScript is running ok!');
<script>
```

**Note:** you can also execute small amounts of code by typing it directly in the console panel and pressing the `Return` Key.

> **< Previous Lesson** ([Lesson 1 - Introduction](https://github.com/evansmwendwa/js-class/blob/master/01-Introduction.md)) **| Next Lesson >** ([Lesson 3 - Syntax](https://github.com/evansmwendwa/js-class/blob/master/03-JS%20Syntax.md))
