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

