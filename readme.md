# Javascript Live Templates for PhpStorm and WebStorm

If you're using PhpStorm on your development, here's some of my customs live templates for javascripts you might wanna use. And also you could import this settings to WebStorm of course.

## What is Live Templates?
Live templates let you insert frequently-used or custom code constructs into your source code file quickly, efficiently, and accurately.

## Installation

Clone this repo

```sh
$ git clone https://github.com/xrexonx/phpStorm-JS-LiveTemplates.git
```

or manually download the zip file on this repo here.



## Installation on your phpStorm
1. On the main menu, choose *File* | *Import Settings*.
2. In the Import File Location dialog box that opens select the desired archive. (it must be the settings.jar)
3. In the Select Components to Import dialog box that opens specify the settings to be imported, and click OK.


#### Restart your phpStorm and then try it on your any javascript file;
empty alert
```javascript
// al
  alert('');
```

return false
```javascript
// rf
  return false;
```

console.log() with parameter response
```javascript
// cl
  console.log(response);
```

empty console.log('') with return false
```javascript
// clr
  console.log(''); return false;
```

console.log() with typeof
```javascript
// clt
  console.log(typeof param);
```

insert use strict statement
```javascript
// us
  "use strict"
```

generating self invoking anonymous function
```javascript
// ()() 
(function () {
    'use strict';
    
    
})();
```

generating named function
```javascript
// fn 
var functionName = function (someParam) {
    //Some awesome code here
}
```

single block of if else condition
```javascript
//ifelse
if (someTrueHere) {

} else {

}
```

if with elseif condition
```javascript
//ifelseif
if () {

} elseif () {

} else {

}
```
switch block statement
```javascript
//sw
switch () {
  case 'strvalue1' :
        //code goes here
        break;
  case 'strvalue2' :
        //code goes here
        break;
  default:
    //code goes here
        break;
    
}
```

create JSON template on your bower.json file
```javascript
//bower
{
  "name": "your-app-name",
    "authors": [
    "Your Fullname here <yourEmail@gmail.com>"
  ],
  "description":"your descriptions",
  "version": "0.0.0",
  "private": true,
  "dependencies": {
    "angular": "1.x",
    "angular-route": "1.x"
  }
}

```

#### Generating javascripts commonly used design patterns.

Object Literal pattern
```javascript
  // olp
var objName = {
  //some property
  myProperty: "someValue",

  // defining further object for module configuration:
  myConfig: {
    useCaching: true,
    language: "en"
  },
 
  // a very basic method
  saySomething: function () {
    //do something awesome here...
  },
  //and more..
 
};
```

Revealing Module Patterns

```javascript
//rmp
var myRevealingModule = (function () {
 
        var privateVar = "Rexon",
            publicVar = "Hey there!";
 
        function privateFunction() {
            console.log( "Name:" + privateVar );
        }
 
        function publicSetName( strName ) {
            privateVar = strName;
        }
 
        function publicGetName() {
            privateFunction();
        }
 
        // Reveal public pointers to
        // private functions and properties
        return {
            setName: publicSetName,
            greeting: publicVar,
            getName: publicGetName
        };
 
    })();
```

#### Thanks and Enjoy. Godspeed! ~xrexonx
