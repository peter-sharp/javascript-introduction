# php-introduction
*An introduction to PHP for those who have been introduced to Javascript

---
PHP is a programming language commonly used in web servers. 
You can switch between php and html by using `<?php` and `?>` tags 


*For this next section we will be using the browser console press command (ctrl) + shift + j to show and hide it*

####Hello world
in PHP:

``` echo 'Hello, world!' ; ```

'echo' is a PHP function that outputs one or more strings. it can be used with or without ( ) braces.

---
##[PHP data types][1]

####Numbers
Same as javascript.

For example:

``` echo 3 * 4 ; ```

**see what other math operations you can do**

####Strings
Same as Javascript

So in 'Hello, world!', 'H' would be at zero. In fact, let's test that using the php string function `indexOf` :

`strros( 'Hello, world!', 'H' );`

###Booleans
Either true or false

###Arrays
Are similar to stings in that they are a sequence but you can store anything you like.
```
array(0,'hi',array('yes even other arrays,', 1), 345 )
```
*[ and ] can also be used*

###objects
a collection of named information and functions that represent a single entity. In PHP these can only be created by 
classes which behave like object factories.
```
class Person {
 $name = 'Dorethy';
 $age = 16;
 $home = false;
}

$dorethy = new Person();
echo dorethy->name;
```
[1]: http://www.cs.utah.edu/~germain/PPS/Topics/data_types.html

##variables
are like little boxes that store information you put inside them

```
$briefcase = 'top secret information';
```

##Control structures
####if statements
Run code between { } braces if a true or truthy value is present in the ( ) braces

```
if( true ) {
  echo('this code will always run');
}
```

commonly used with:
 + > greater than
 + < less than
 + === equal to

if you want something else to happen when if is not true use *else*

```
if( false ) {
  echo('this will never run');
} else {
  echo('But this will!!!');
}
```

####for loops
run the code between the { } braces until the condition is met

```
for($i = 0; $i < 100; $i++){
 echo( $i . ' bottles of beer on the wall' );
}
```

####foreach loops
loop over each item in an array

```
$navItems = array('home', 'about', 'products', 'contact');
```

```
foreach( $navItems as $navItem ){
  echo '<a href="#">'.$navItem.'</a>';
}
```

##functions
Named ( or anonymous) blocks or code you can run at any time. They can take a list of values called parameters. Functions can optionally return a value as well.

```
function greet() {
  echo 'Hi there!' ;
}
```


```
function cubed( number ) {
  return number * number * number;
}
```

