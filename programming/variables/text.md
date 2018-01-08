### Variables

>Variables are used to store information to be referenced and manipulated in a computer program. They also provide a way of labeling data with a descriptive name, so our programs can be understood more clearly by the reader and ourselves. It is helpful to think of variables as containers that hold information. Their sole purpose is to label and store data in memory. This data can then be used throughout your program. <sub>--https://launchschool.com/books/ruby/read/variables</sub>

The following statement _declares_ a variable named `v` and _assigns_ it a value `5`:
```python
v = 5
``` 

If you enter the above statement in the interactive shell in order to cause the shell to remember the variable name `v` and its value. 
```
>>> v = 5
>>> 
```
Now, you can cause the shell to recall the value by simply typing in the variable name as an expression.
```
>>> v
5
>>> 
```
You can even use the variable in expressions.
```
>>> v * 4
20
>>>
```

Here are some more examples:

```python
max_bag_count = 2
price = 10.50
is_new = True
```

<tip-box> 

**Variable names**

Python variable names typically use lower case letters with `_` separating words. 
```python
long_variable_name = 56
```

Variable names are case sensitive. In the example below, you can see how Python prints an error message if you try to access the variable `height` using the name `Height`
```
>>> height = 12.0
>>> height
12.0
>>> Height
Traceback (most recent call last):
 File "< pyshell#5 >", line 1, in < module >
   Height
NameError: name 'Height' is not defined
``` 
</tip-box>

**Variables can be reassigned**. In the example below, `height` was initially 5 but the value is reassigned later to be 1 more than the previous value.

```
>>> height = 5
>>> height
5
>>> height = height + 1
>>> height
6
>>> 
```

**Value of one variable can be assigned to another variable.** In the example below, the value of variable `height` is assigned to the variable `width`.
```
>>> height = 5
>>> width = height
>>> width
5
>>> height + width
10
>>> height = 10
>>> width
5
```