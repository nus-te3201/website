### Using Functions

**A _function_ is like a small program that you can execute from another program. A function has a name and might take some inputs** (called _parameters_ or _arguments_). The statement to _execute_ (other names: _call_, _invoke_) a function takes the form `function_name(parameters)` %%&nbsp;e.g., `foo(1, 'hello')` calls a function named `foo` with parameters `1` and `'hello'`%% 

Python comes with many built-in functions you can use right away. 

:package: To find the type of a value, you can use the built-in function `type`.
```
>>> type(-4)
< class 'int' >

>>> type(44.0)
< class 'float' >

>>> type('hello')
< class 'str' >
```

:package: To print some content, you can use the `print` function which can take one or more string arguments:

```
>>> print('Hello World')
Hello World

>>> print ('Bye', 'my', 'friend')
Bye my friend
```

:bulb: A call to `print` without any arguments (i.e. `print()`) prints an empty line.

**Some functions return a value.**

:package: `int`, `float`, `str` functions can be used to convert a data of one type to another.

```python
age = 25
print('My age is ' + str(age))
```

:package: `input` function can be used to read input from the keyboard. It waits for user input (until the user hits <kbd>Enter</kbd>) and returns all text entered by the user ==as a string==.

```python
# read current price
print('What is the current price?')
price = input()

# print current price
print() # print an empty line
print('Current price is $' + price)

# calculate and show discounted price
discounted_price = float(price)*0.5
print('Price after 50% discount is $' + str(discounted_price))
```

<panel type="seamless" header="%%:arrow_forward: Try above code online%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/discounted?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>

<panel type="seamless" header="%%:tv: Explanation of a small Python program%%">

<iframe width="560" height="315" src="https://www.youtube.com/embed/buMTH6ICnqk?rel=0&showinfo=0&start=169&version=3" frameborder="0" allowfullscreen></iframe>

</panel>