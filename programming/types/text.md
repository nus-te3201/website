### Data Types

A data value has a _type_. 

Here is a summary of three basic data types used in Python often.

Type name | Description | Examples 
--------- | ----------- | ------
`int` | whole numbers (integers) |  `-23` `-22`  `-1` `0` `1` `65` `66`
`float` | numbers with decimal points (floating point numbers) |  `-34.576`  `436.0` 
`str` | sequence of characters (strings) | `adam` `What can it be?` `x`


String values are denoted by enclosing them in double quotes or single quotes.

```
'Hello'
"What's going on?"
```

Some operators can be used on strings as well.
```
>>> 'hello'
'hello'
>>> 'Hello' + ' ' + 'World!'
'Hello World!'
>>> 'Bye' + ('!' * 10)
'Bye!!!!!!!!!!'
```

To find the type of a value, you can use the built-in function `type()`.
```
>>> type(-4)
< class 'int' >
>>> type(44.0)
< class 'float' >
>>> type('hello')
< class 'str' >
```

<panel type="seamless" header="%%:tv: Data types%%">

<iframe width="560" height="315" src="https://www.youtube.com/embed/7qHMXu99d88?rel=0&start=317&end=416&version=3" frameborder="0" allowfullscreen></iframe>

</panel>