# javascript-introduction
*An introduction to Javascript for those who have been introduced to HTML, CSS (, and perhaps toyed with a bit of jQuery )*

---
Javascript is a programming language commonly used in web browsers to add dynamic and interactive features to web pages. Ever wondered how the webpage knew you hadn't entered a correct email address before you submitted the form? Javascript. Form validation is just one example of javascript can do, you can create all sorts of [apps](http://todomvc.com/examples/vanillajs/) and [games](http://www.jsbreakouts.org/phaser/index.html) using the language.

*For this next section we will be using the browser console press command (ctrl) + shift + j to show and hide it*

####Hello world
A "hello world" program shows the basic syntax ( computer language grammar ) needed for a working computer program.
in javascript this is:

``` alert( 'Hello, world!' ); ```

'alert' is a javascript function ( we'll get to functions later ) that tells your web browser to display a popup window with some text you give it in quotes.

---
##[Javascript data types][1]

####Numbers
Javascript can be used to do basic math operations with numbers.

For example:

``` alert( 3 * 4 ); ```

**see what other math operations you can do**

####Strings
Javascript and other computer programming languages store text as a sequence of characters called a string. Each position in a string has a number index *starting from zero*, **important to remember**.

So in 'Hello, world!', 'H' would be at zero. In fact, let's test that using the Javascript string function `indexOf` :

`'Hello, world!'.indexOf('H');`

###Booleans
Either true or false

###Arrays
Are similar to stings in that they are a sequence but you can store anything you like.
```
[0,'hi',['yes even other arrays,', 1], 345 ]
```

###Objects
a collection of named information and functions that represent a single entity.
```
{
 name: 'Dorethy',
 age: 16,
 home: false
}
```
[1]: http://www.cs.utah.edu/~germain/PPS/Topics/data_types.html

##variables
are like little boxes that store information you put inside them

```
var briefcase = 'top secret information';
```

##Control structures
####if statements
Run code between { } braces if a true or truthy value is present in the ( ) braces

```
if( true ) {
  console.log('this code will always run');
}
```

commonly used with:
 + > greater than
 + < less than
 + === equal to

if you want something else to happen when if is not true use *else*

```
if( false ) {
  console.log('this will never run');
} else {
  alert('But this will!!!');
}
```

####for loops
run the code between the { } braces until the condition is met

```
for(var i = 0; i < 100; i++){
 console.log( i + ' bottles of beer on the wall' );
}
```

A more advanced example:

```
var nav_items = document.querySelectorAll('.reponav-item');
```

```
for( var i = 0; i < nav_items.length; i++){
 var nav_item = nav_items[i];
console.log( nav_item.innerHTML );
}
```

##functions
Named ( or anonymous) blocks or code you can run at any time. They can take a list of values called parameters. Functions can optionally return a value as well.

```
function greet() {
  alert('Hi there!');
}
```


```
function cubed( number ) {
  return number * number * number;
}
```

