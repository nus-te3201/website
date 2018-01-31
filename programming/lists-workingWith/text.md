### Working with Lists

**You can use the _slice_ notation `list_name[start_index:end_index]` to get a _<tooltip content="get a portion of the list as a new list">sublist</tooltip>_.**

<tip-box> 

:package: Some example of slicing to get a sub list:
  
```python
letters = ['0a', '1b', '2c', '3d', '4e']
print(letters[0:3]) # print items 0, 1, 2
print(letters[:3]) # same as above (first 3 items)
print(letters[1:4]) # print items 1, 2, 3
print(letters[3:]) # print from item 3 till end
print(letters[-2:]) # print last two items
print(letters[1:-1]) # print from item 1 to 2nd last item
```
:arrow_heading_down:
```
['0a', '1b', '2c']
['0a', '1b', '2c']
['1b', '2c', '3d']
['3d', '4e']
['3d', '4e']
['1b', '2c', '3d']
```
<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-slicing?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

</tip-box>

Note that slicing gives you a _copy_ of a portion of the original list i.e., you get a new list.


<tip-box> 

:package: In the example below, the first item `0a` of the list `letters` is deleted after taking the first two elements as a sub list. Note how the item `0a` still remains in the sub list after it has been deleted from the original list.
  
```python
letters = ['0a', '1b', '2c', '3d', '4e']
first_two_letters = letters[:2]
print('original list:', letters)
print('sub list     :', first_two_letters)
del letters[0] # delete first element in original list
print('original list:', letters)
print('sub list     :', first_two_letters)
```
:arrow_heading_down:
```
original list: ['0a', '1b', '2c', '3d', '4e']
sub list     : ['0a', '1b']
original list: ['1b', '2c', '3d', '4e']
sub list     : ['0a', '1b']
```
<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-slicing?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

</tip-box>