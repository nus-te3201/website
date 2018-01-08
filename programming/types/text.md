### Data Types

A data value has a _type_. In the example below, `max_bag_count` is assigned an _integer_ number, `price` is assigned a _floating point_ number, and `is_new` is assigned a _boolean_ value.
```python
max_bag_count = 2
price = 10.50
is_new = True
```

Here is a summary of three basic data types used in Python often.

Type name | Description | Values 
--------- | ----------- | ------
`int` | whole numbers | ..., -23, -22, ..., -1, 0, 1, ... 65, 66, ...
`float` | floating point numbers | ..., -34.576, ..., 436.0, 
`bool` | boolean values | `True`, `False`

To find the type of a value, you can use the built-in function `type()`.
```
>>> type(-4)
<class 'int'>
>>> type(44.0)
<class 'float'>
>>> type(False)
<class 'bool'>
```

**Python is a _dynamically typed_ language.** That means a value has a type %%&nbsp;e.g., `int`, `float`, `bool` etc.%%  but the variable itself does not have a type. The variable takes the type of whatever value it holds. Note how the type of `x` changes from `int` to `float` in the example below.
```
>>> x = 3
>>> type(x)
<class 'int'>
>>> x = 34.5
>>> type(x)
<class 'float'>

```

<panel type="seamless" header="%%_Statically typed_ languages%%">

In contrast, a variable in a _statically typed_ language (e.g., Java) has a type and the type of a variable cannot change over time. For example, an integer variable cannot hold a boolean values later.

</panel><p/>

Another very frequently used data type is strings (Python name: `str`). String values are denoted by enclosing them in double quotes or single quotes.

```python
husband = 'John Doe'
wife = "Jane Doe"
description = "This hasn't been done yet!"
```