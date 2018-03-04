### Reading from Files

This section focuses on reading from text-based files (i.e., not binary files).

**There are three steps to reading or writing files in Python:**
* Call the **`open()`** function to receive `File` object.
* Call the **`read()`** method on the `File` object to receive file content.
* Close the file by calling the **`close()`** method on the `File` object.

<tip-box> 

:package: The code below shows how to read from a text file.

<table> 
<tr>
  <td>

```python
file_path = os.path.join('data', 'items.txt')
f = open(file_path, 'r') # open in read mode
items = f.read()
print(items)
f.close()
```
  </td>
  <td><br><br>&nbsp;→&nbsp;</td>
  <td><br><br>
Output (contents of the `items.txt`):
```
first line
second line
third line
```
  </td>
</tr>
</table>

:bulb: The `'r'` argument in `open(file_path, 'r')` indicates that the file should be opened in read mode. 

</tip-box>

It is also possible to read the file content as a list of lines, using the `readlines()` method.

<tip-box> 

:package: The code below shows how to read file content as a list of lines.

```python
f = open(file_path, 'r')
items = f.readlines()
print(items) # print as a list
for i in items: # print each item
  print(i.strip()) # strip to remove linebreak
f.close()
```
:arrow_heading_down:
```
['first line\n', 'second line\n', 'third line\n']
first line
second line
third line
```
:bulb: Note how each line ends with a `\n` which represents the line break. It can be removed using the `strip()` method.

</tip-box>