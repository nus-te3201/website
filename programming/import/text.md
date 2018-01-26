### Importing Modules

**A Python _module_ is a python program that contains a related group of functions**. You can think of it as a file containing some python functions.

In addition to built-in functions such as `print()`, `input()`, and `len()`, **Python also comes with a set of modules called the _standard library_.** 

<tip-box> 

:package: Some example modules in the Python standard library:

Name | What it contains
---- | ----------------
`math` | mathematics-related functions
`random` | random number–related functions
`sys` | provides ways to interact with the Python interpreter

</tip-box>
 
Unlike built-in functions which you can use simply use in your code, **to use a function in the standard library you need to _import_ the module first.**

Format: `import module_name(s)`

:package: Some examples:
* `import math`
* `import math, sys, random`

Furthermore, to use a function from an imported module, you should use the `module_name.function_name()` format.

<tip-box>

:package: the code below imports the `random` module and uses its `randint()` function to generate a number between 1 and 10. 


```python
import random

print('Going to print 5 random numbers between 1 and 10')
for i in range(5):
    print(random.randint(1, 10))
```

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/five-randoms?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

</tip-box>

:bulb: It is common practice to put the `import` statements at the top of the program code.
