#### Exercise : Delete Head, Delete Tail

Complete the functions as described below:
* `delete_head(item_list)`: deletes the first item in the list passed as `item_list` parameter.
* `delete_tail(item_list)`: deletes the last item in the list passed as `item_list` parameter.

:bulb: `pass` is a dummy statement that does nothing. We use it here because Python does not accept empty functions.

<table>
<tr>
  <td>

```python
def delete_head(item_list):
  pass # delete this dummy statement
  
def delete_tail(item_list):
  pass # delete this dummy statement
  
letters = ['a', 'b', 'c']
print(letters)
delete_head(letters)
print(letters)
delete_tail(letters)
print(letters)
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```









['a', 'b', 'c']
['b', 'c']
['b']

```
  </td>
</tr>
</table>