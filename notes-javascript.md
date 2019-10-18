### Chapter Content
 - **Chapter 1** - looks at some key concepts in computer programming, showing you how computers create models of the world using data, and how JavaScript is used to change the contents of an HTML page.
- **Chapters 2-4** cover the basics of the JavaScript language.
- **Chapter 5** explains how the Document Object Model (DOM) lets you access and change a document's contents while it is loaded into the browser.
- **Chapter 6** discusses how events can be used to trigger code.
- **Chapter 7** shows you how jQuery can make the process of writing scripts faster and easier.
- **Chapter 8** introduces you to Ajax, a set of techniques that allow you to just change part of a web page without reloading the entire page.
- **Chapter 9** covers Application Programming Interfaces (APls), including new APls that are part of HTMLS and those of sites like Google Maps.
PRACTICAL A PPLICATIONS
By this point you will already have seen many examples of how JavaScript is used on popular websites. This section brings together all of the techniques you have learned so far, to give you practical demonstrations of how JavaScript is used by professional developers. Not only will you see a selection of in-depth examples, you will also learn more about the process of designing and writing scripts from scratch.
- **Chapter 10** deals with error-handling and debugging, and explains more about how JavaScript is processed.
- **Chapter 11** shows you techniques for creating content panels-such as sliders, modal windows, tabbed panels, and accordions.
- **Chapter 12** demonstrates several techniques for filtering and sorting data. This includes filtering a gallery of images, and re-ordering the rows of a table by clicking on the column headings.
- **Chapter 13** deals with form enhancements and how to validate form entries.

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


##### Chapter 1
- Access Content
- Modify Content
- Program Rules
- React to Events

- JavaScript can reload only portions of the website instead of the entire page so that it functions more like an app and not a web page.
- Can be used as a filter.

#### Comparison Operators: Evaluating Conditions (Page 150)
`==` is equal to
`===` strict equal to
`!=` is not equal to
`!==` strict not equal to

`>` greater than
`>=` greater than or equal to
`<` less than
`<=` less thn or equal to

#### Logical Operators (Page 156-157)
`((5 < 2) && (2 >= 3))`
`&&` is the logical operator
`(5 < 2)` is `false`
`(2 >= 3)` is `false`
Therefore the equation evaluated is `(false) && (false)`
The `&&` is the third evaluation/expression and asks if both expressions are true or not. In this case, both are `false` so the last evaluation/expression is `false`.

`||` logical or (does at least one expression/evaluation return true? If so, then `true`.
`!` logical not (does the expression following the operator equal NOT true/false? if so, then `true`) `!(2 < 1)` this returns `true`
