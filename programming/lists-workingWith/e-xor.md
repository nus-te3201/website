#### Exercise : XOR

%%:book: In case you didn't know: _XOR_ (short for eXclusive OR) is a logical operation, when applied to two booleans, that outputs true only when inputs differ (one is true, the other is false)%%

Complete the functions as described below:
* `xor(list1, list2, item)`: returns `True` if `item` is in ++only++ one of the two lists `list1` and `list2`. i.e., returns `False` if the `item` is absent from both lists or present in both lists.


<table>
<tr>
  <td>

```python
def xor(list1, list2, item):
  return

print(xor(['a','b'], ['a', 'c'], 'a'))
print(xor(['a','b'], ['a', 'c'], 'b'))
print(xor(['a','b'], ['a', 'c'], 'c'))
print(xor(['a','b'], ['a', 'c'], 'd'))
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```



False
True
True
False

```
  </td>
</tr>
</table>