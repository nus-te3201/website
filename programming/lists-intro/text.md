### The List Data Structure

**A _data structure_ contains data that are more complex than a single data value** such as an integer. Lists are one such very useful data structure in Python. **A list contains a sequence of _items_.** Python uses square brackets to indicate lists.

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

**You can use the notation `list_name[index_of_item]` to access items of a list.** List indexes start from `0` i.e., the first item in a list has the index `0`.

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

:bulb: As you can see from the above example, you can use negative indexes too; index `-1` refers to the last item in the list, `-2` refers to the second last item in the list, and so on.

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

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-access-using-index?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

</tip-box>

**You can use `del` to delete an item from a list.**

<tip-box>

:package: The code below shows how to use `del` to delete items in a list.

<table>
<tr>
  <td>
  
```python
spam = ['foo', 45.0, True]
del spam[-1]
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

**You can use `len` function to find the number of items in a list** %%&nbsp;e.g., `len(['a','b'])` evaluates to `2` as the list has 2 items%%.