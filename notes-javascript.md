### JavaScript Notes
- Action - Logic in code.
    - on page load
    - user interaction

### In Class Code Example

##### add-content.html
```
<!DOCTYPE html>
<html>
    <head>
        <title>Constructive &amp; Co. </title>
        <link rel="stylesheet" href="css/c01.css">
    </head> 
    <body>
        <h1>Constructive &amp; Co.</h1>
        <script src="js/add-content.js"></script> 
        <p>For all orders and inquiries please call
            <em>555-3344</em></p> 
    </body>
</html>
```

##### add-content.js
```
'use strict';

var today = new Date();
var hourNow = today.getHours();
var greeting;

if (hourNow > 18) {
    greeting = 'Good evening!';
} else if (hourNow > 12) {
    greeting = 'Good afternoon!';
} else if (hourNow > 0) {
    greeting = 'Good morning!';
} else {
    greeting = 'Welcome!';
}

document.write('<h3>' + greeting + '</h3>');
```