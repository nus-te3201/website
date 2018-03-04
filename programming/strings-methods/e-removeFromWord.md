#### Exercise : Remove From Word

Complete the `remove_from_word` function given below, to behave as follows:
* If `text` is all upper case, return `text` in lower case
* If `text` is all lower case, return `text` in upper case
* Return `text` otherwise

```python
def remove_from_word(text, tail_start_word):
  #pass # REPLACE WITH YOUR CODE

```

Example usage:
<table> 
<tr>
  <td>

```python
print('>' + remove_from_word('red-hot-lava', 'red'))
print('>' + remove_from_word('red-hot-lava', 'hot'))
print('>' + remove_from_word('red-hot-lava', 'lava'))
```
  </td>
  <td><br>&nbsp;→&nbsp;</td>
  <td><br>

```
>
>red-
>red-hot-
```
  </td>
</tr>
</table>


<panel type="seamless" header="%%:bulb: Partial solution%%">

```python
def remove_from_word(text, tail_start_word):
  tail_start_position = text.find(tail_start_word)
  if tail_start_position != -1:
    return ...
  else:
    return ...
```

</panel>