# CSS Notes
- There are **Selectors** `p {font-family: Arial;}` "p" is the selector.
>**Selectors** indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas. 
- There are declarations `p {font-family: Arial;}` "{font-family: Arial;}" is the declaration.
>**Declarations** indicate how
the elements referred to in the selector should be styled. **Declarations** are split into two parts (a property and a value), and are separated by a colon.
- There are **values**. "Arial" or "Yellow" are the **values**.
> **Values** specify the settings
you want to use for the chosen properties. For example, if you want to specify a color property then the value is the color you want the text in these elements to be.

##### Internal CSS Example
- `<!DOCTYPE html>
<html>
<head>
<title>Using Internal CSS</title> <style type="text/css">
      body {
          font-family: arial;
          background-color: rgb(185,179,175);}
      h1 {
          color: rgb(255,255,255);}
    </style>
  </head>
<body>
<h1>Potatoes</h1>
<p>There are dozens of different potato
       varieties. They are usually described as
early, second early and maincrop.</p> </body>
</html>`

##### External CSS Example
- HTML File (file.html)
```<!DOCTYPE html>
<html>
<head>
<title>Using External CSS</title>
<link href="css/styles.css" type="text/css"
      rel="stylesheet" />
  </head>
<body>
<h1>Potatoes</h1>
<p>There are dozens of different potato
       varieties. They are usually described as
early, second early and maincrop.</p> </body>
</html>```

- CSS file (styles.css)
```body {
    font-family: arial;
    background-color: rgb(185,179,175);}
h1 {
    color: rgb(255,255,255);}```


