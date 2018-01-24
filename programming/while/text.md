### Flow Control Using `while`

Python uses the `while` statement to repeat a code block until a certain condition is true.

Format:
```
while condition :
    statements_to_execute_if_condition_is_true
```

:package: the code below prints 'Hello' 3 times, followed by 'Done'.
```python
counter = 0
while counter < 3:
    print('Hello')
    counter = counter + 1
print('Done')
```
Output :arrow_heading_down: <trigger trigger="click" for="modal:multipleHello-pyTutor">%%[Click here to visualize execution]%%</trigger>
```
Hello
Hello
Hello
Done
```
<modal large title="Code with a simple `if` condition" id="modal:multipleHello-pyTutor">

<iframe width="800" height="500" frameborder="0" src="http://pythontutor.com/iframe-embed.html#code=counter%20%3D%200%0Awhile%20counter%20%3C%203%3A%0A%20%20%20%20print%28'Hello'%29%0A%20%20%20%20counter%20%3D%20counter%20%2B%201%0Aprint%28'Done'%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=10&heapPrimitives=false&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

</modal>

.. more content to be added

