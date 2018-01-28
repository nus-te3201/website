### Function Arguments

**You can configure a function to take arguments**. The arguments can be used by the code inside the function. That means we can use arguments to affect the behavior of a function so that the function behaves differently each time it is executed. 

Format:
```
def function_name(argument1_name, argument2_name, ...):
    ...
```

<tip-box> 

:package: The `say_hello` function below takes one argument.

<table>
<tr>
  <td>
  
```python
def say_hello(name):
  print('Hello ' + name)
  print('How are you', name, '?')
  
say_hello('Gina')
say_hello('John')
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```
Hello Gina
How are you Gina ?
Hello John
How are you John ?



```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/hello-name?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

:package: The code below has one function that takes one argument and one that takes two. Furthermore, note how one function calls the other.

```python
def say_hello(name):
  print('Knock knock ' + name)

def repeat_hello(name, times):
  print('Greeting ', name, times, 'times')
  for i in range(times):
    say_hello(name)
  
repeat_hello('Penny', 3)
say_hello('Sheldon')
```

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/hello-given-times?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

<panel type="seamless" header="%%:laughing: See human version of the above code%%">
<iframe width="560" height="315" src="https://www.youtube.com/embed/jrzUsHNGZHc?rel=0&showinfo=0&start=0&end=15&version=3" frameborder="0" allowfullscreen></iframe>

</panel><p/>

</tip-box>

**Parameter values are are forgotten after the function returns**.

<tip-box> 

:package: The code below produces an error because argument `v1` is not available after the function has returned.

```python
def print_uniqueness(v1, v2, v3):
  print(v1 != v2 and v2 != v3 and v3 != v1)
  
print_uniqueness(1,2,4) # True
print_uniqueness(1,1,2) # False

# Error. v1 is not available after function returns
print(v1) 
```

</tip-box>