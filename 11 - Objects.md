## JavaScript Objects

Objects are variables that contain many values
Arrays are types of Objects

#### Example Object

``` javascript
var car = {
  type:"Fiat", 
  model:"500", 
  color:"white"
};
```

The values are written as name:value pairs (name and value separated by a colon).

> JavaScript objects are containers for named values.

### Object Properties

The name:values pairs (in JavaScript objects) are called properties.

``` javascript
var person = {
  firstName:"John", 
  lastName:"Doe", 
  age:50, 
  eyeColor:"blue"
};
```
### Object Methods

Methods are actions that can be performed on objects.

Methods are stored in properties as function definition

> JavaScript objects are containers for named values called properties or methods.

``` javascript
var person = {
  firstName:"John", 
  lastName:"Doe", 
  age:50, 
  getName: function() {
    return "John" + " " + "Doe";
  }
};
```

### Accessing Object Properties

You can access object properties in two ways:
```
objectName.propertyName
```
or 
``` javascript
objectName["propertyName"]
```
**Example 1**
``` javascript
person.lastName;
```

**Example 2**
``` javascript
person["lastName"];
```

### Accessing Object Methods
You access an object method with the following syntax:
```
objectName.methodName()
```

**Example**
```
name = person.fullName();
```

> If you access the fullName method, without (), it will return the function definition:

``` javascript
name = person.fullName;
```

### Do Not Declare Strings, Numbers, and Booleans as Objects!

When a JavaScript variable is declared with the keyword "new", the variable is created as an object:

```
var x = new String();        // Declares x as a String object
var y = new Number();        // Declares y as a Number object
var z = new Boolean();       // Declares z as a Boolean object
```

> Avoid String, Number, and Boolean objects. They complicate your code and slow down execution speed.
