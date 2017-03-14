## JavaScript statements

All the JavaScript code that you will write will, for the most part, be comprised of many separate statements. A statement can set a variable equal to a value. A statement can also be a function call, i.e. document.write(). Statements define what the script will do and how it will be done.

## Categories of statements

In addition to standard statements like changing a variable's value, assigning a new value, or calling a function, there are groups of statements that are distinct in their purpose. We will provide a brief overview of each of these categories in this lesson and cover them in greater detail later in the tutorial. These distinct groups of statements include:

* Conditional Statements
* Loop Statements
* Object Manipulation Statements
* Comment Statements
* Exception Handling Statements

## Conditional statements

If you were to win a $100 million lottery, you would probably quit your job. That last statement is a conditional if/then statement that is used a great deal in programming. If some condition (winning the lottery) is true, then something happens (you quit your job). If the condition is false (you didn't win the lottery), then you probably will not take that action (quit your job).

Conditional statements are used to control your scripts so that different actions can be taken depending on the situation. You may want to display a special image on your home page during the holidays. This condition would depend on what day it was, and if it was a holiday, then a special holiday image would be displayed to your visitors. Without proper knowledge of the conditional statement, your scripts will not be as lively or dynamic as they could possibly be.

## Loop statements

A loop statement checks to see if some condition is true, and if that condition is true, it executes a chunk of code. After the code is executed, the condition is checked again. If it is true, the process starts over again; if it is false, the loop stops and the rest of the code continues along. If we think about our wedding invitation example as a loop, we would first check if there are any invitations left. If there are, we would stuff, lick, and seal the next envelope. If there are no envelopes left, we would stop.

## Comment statements

Comment statements are used to prevent the browser from executing certain parts of code that you designate as non-code. Why would you want to do this? There are many reasons. By disallowing the block of text from being be read, you can then place in comments for yourself, much like HTML comments. You can also block out segments of your code for whatever reason you may have.

The single line comment is just two slashes (//) and the multiple line comment starts with (/*) and ends with (*/). We will talk about comments in greater depth in a later lesson.

## Exception handling statements

Sometimes when you are programming you do not know for sure if the file that you will be writing to, the input stream you are reading from, or the connection you have established will be usable for the code that you want to execute. There is a way to program safety mechanisms, so that your code handles common problems that may arise (maybe the input stream you are reading from suddenly disappears).

The try...catch statement tries to execute a piece of code and if it fails, the catch should handle the error gracefully. This is an advanced programming subject that is interesting, but not necessary for the majority of JavaScript programmers.
