##What is a function?

A function is a piece of code that sits dormant until it is referenced or called upon to do its "function".
In addition to controllable execution, functions are also a great time saver for doing repetitive tasks.

Instead of having to type out the code every time you want something done, you can simply call the function multiple times to get 
the same effect. This benefit is also known as "code reusability".

##Example Function in JavaScript
Creating a function is really quite easy. All you have to do is tell the browser you're making a function, give the function a name, 
and then write the JavaScript like normal. Below is the example alert function from the previous lesson.

``` html
<html>
    <head>
        <script type="text/javascript">
        function popup() {
            alert("Hello World")
        }
        </script>
    </head>
    <body>
    <button onclick="popup()">Popup</button>
    </body>
</html>
```

We first told the browser we were going to be using a function by typing "function". Next, we gave our function a name, 
so that we could use it later. Since we are making a pop up alert, we called our function "popup".

The curly braces "{,}" define the boundaries of our function code. All popup function code must be contained within the curly braces.

Something that might be slightly confusing is that within our "popup" function, we use another function called "alert," 
which brings up a popup box with the text that we supply it. It is perfectly OK to use functions within functions, like we have done here.

In order to get the function executed when we click the button we used the `click`. The click is called an event. There are many types of events that represent different user interactions with your web page.

##Events in JavaScript
The building blocks of an interactive web page is the JavaScript event system. An event in JavaScript is something that happens with or on the webpage. A few example of events:

* A mouse click
* The webpage loading
* Mousing over a hot spot on the webpage, also known as hovering
* Selecting an input box in an HTML form
* A keystroke

##Examples using Events

JavaScript has predefined names that cover numerous events that can occur, including the ones listed above. To capture an event and make something happen when that event occurs, you must specify the event, the HTML element that will be waiting for the event, and the function(s) that will be run when the event occurs.

We have used a JavaScript event in a previous lesson, where we had an alert popup when the button was clicked. This was an "onclick" JavaScript event. We will do that same example again, as well as the mouseover and mouseout events.

``` html
<html>
  <head>
    <script type="text/javascript">
    function popup() {
	    alert("Hello World")
    }
    </script>
  </head>
  <body>
    <button type="button" onclick="popup()">Click Me!</button>
    <br />
    <a href="#" onmouseover="" onMouseout="popup()">Hover Me!</a>
  </body>
</html>
```

With the button we used the event onClick event as our desired action and told it to call our popup function that is defined in our header. To call a function you must give the function name followed up with parenthesis "()".

Our mouseover and mouseout events were combined on one HTML element--a link. We wanted to do nothing when someone put their mouse on the link, but when the mouse moves off the link (onMouseout), we displayed a popup.
