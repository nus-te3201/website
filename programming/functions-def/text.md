### Writing Functions

**You can write your own functions in Python.** Function are useful when you want to execute a bunch of statements multiple times at different points of a program. 

Format:
```
def function_name():
    statement_1
    statement_2
    ...
```

<tip-box> 

:package: The code below defines a function named `say_hello` and calls it twice.

<table>
<tr>
  <td>
  
```python
def say_hello():
  print('Hello!')
  print('How are you?')
  print('Nice to meet you.')
  
# call the function twice
print('Going to call the function ...')
say_hello()
print('Going to repeat ...')
say_hello()
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```
Going to call the function ...
Hello!
How are you?
Nice to meet you.
Going to repeat ...
Hello!
How are you?
Nice to meet you.



```
  </td>
</tr>
</table>

Note how the statements inside the function are not executed unless the method is called. 

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/hello-function?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

</tip-box>

The function definition should appear in the code _before_ it is called.
 
<tip-box> 

<table>
<tr>
  <td>

:+1: this works
```python
print('starting ...')

def say_hello():
  print('Hello!')

print('Going to say hello ...')

say_hello()

```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
:-1: this doesn't work
```python
print('starting ...')

# call appears before definition
say_hello() 

def say_hello():
  print('Hello!')

print('Going to say hello ...')
```
  </td>
</tr>
</table>

</tip-box>
