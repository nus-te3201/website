### The List Data Structure

**A _data structure_ contains data that are more complex than a single data value** such as an integer. Lists are one such very useful data structure in Python. **A list contains an ordered sequence of _items_.** Python uses square brackets to indicate lists.

<tip-box> 

:package: Some list examples:
  
```python
friends = [] # an empty list
fruits = ['apple', 'banana', 'orange'] # a list containing 3 string items
values = [0, 3.4, 'High', True] # a list containing items of different types
print(friends, fruits, values)

everything = [friends, fruits, values] # a list containing other lists
print(everything)
```
:arrow_heading_down:
```
[] ['apple', 'banana', 'orange'] [0, 3.4, 'High', True]
[[], ['apple', 'banana', 'orange'], [0, 3.4, 'High', True]]
```
</tip-box>

<panel type="seamless" header="%%:tv: Lists%%">
<iframe width="560" height="315" src="https://www.youtube.com/embed/5n6o1MaXDoE?rel=0&showinfo=0&start=11&end=70&version=11" frameborder="0" allowfullscreen></iframe>

</panel><p/>

**You can use the notation `list_name[index_of_item]` to access an item of a list.** List indexes start from `0` i.e., the first item in a list has the index `0`.

<tip-box>

:package: The code below shows how to use indexes to access items in a list.

<table>
<tr>
  <td>
  
```python
fruits = ['Apple', 'Banana', 'Cherry', 'Dragon fruit']
print(fruits[0])
print(fruits[3])
print(fruits[-1])
print(fruits[-2])
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```

Apple
Dragon Fruit
Dragon Fruit
Cherry

```
  </td>
</tr>
</table>

:bulb: As you can see from the above example, **list indexes can be negative**; index `-1` refers to the last item in the list, `-2` refers to the second last item in the list, and so on.

:package: The code below shows how to use indexes to update items in a list.

<table>
<tr>
  <td>
  
```python
coins = [10, 30, 50, 100]
coins[1] = 20
print(coins)
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```


[10, 20, 50, 100]

```
  </td>
</tr>
</table>

:package: The example below shows how to access an item of a list that is inside another list; `list_of_lists[2]` accesses `list_of_lists[2]` which gives you the item at index 2 (`[0.1, 0.2]`) which is also a list, and then accesses the item at index `0` from that list, which is `0.1`. 

<table>
<tr>
  <td>
  
```python
list_of_lists = [['a', 'b', 'c'], [1, 2, 3, 4], [0.1, 0.2]]
print(list_of_lists[2][0])
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```

0.1

```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-access-using-index?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

</tip-box>

<panel type="seamless" header="%%:tv: Accessing an item from a list%%">
<iframe width="560" height="315" src="https://www.youtube.com/embed/5n6o1MaXDoE?rel=0&showinfo=0&start=70&end=317&version=11" frameborder="0" allowfullscreen></iframe>

</panel><p/>

**You can use the _slice_ notation `list_name[start_index:end_index]` to copy a _<tooltip content="a portion of a list">sublist</tooltip>_ into a new list.**

<tip-box> 

:package: Some example of slicing to get a sub list:
  
```python
letters = ['0a', '1b', '2c', '3d', '4e']
sublist = letters[0:3]
print(sublist]) # print items 0, 1, 2
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

</tip-box>

<panel type="seamless" header="%%:tv: Accessing multiple items from a list%%">
<iframe width="560" height="315" src="https://www.youtube.com/embed/5n6o1MaXDoE?rel=0&showinfo=0&start=317&end=534&version=11" frameborder="0" allowfullscreen></iframe>

</panel><p/>

**You can use `del` to delete an item at a specific position of a list.**

<tip-box>

:package: The code below shows how to use `del` to delete items in a list.

<table>
<tr>
  <td>
  
```python
spam = ['foo', 45.0, True]
del spam[-1] # delete last item
print(spam)
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```


['foo', 45.0]

```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-access-using-index?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

</tip-box>

<panel type="seamless" header="%%:tv: Deleting items from a list%%">
<iframe width="560" height="315" src="https://www.youtube.com/embed/5n6o1MaXDoE?rel=0&showinfo=0&start=534&end=581&version=11" frameborder="0" allowfullscreen></iframe>

</panel><p/>