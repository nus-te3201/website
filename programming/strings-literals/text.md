### String Literals

A <tooltip content="a string value, not a variable">string literal</tooltip> can normally be specified by enclosing it within a pair of `''` or a pair of `""` %%e.g., `'How is life?'`%%. However, this will not work if the string has a <tooltip content="a character that has special meaning in Python">special character</tooltip> in it %%e.g., `'How's life?'` is not acceptable to Python because it contains a `'` which has the special meaning 'end of string', confusing Python as to which `'` of the string literal indicates the end of the string. This is similarly confusing: `"Say "wow""`%%.

You can **use the `\'` _escape sequence_  to have a `'` in strings**. An escape sequence is a sequence of characters in a string literal that is taken together and interpreted in a special way. Given below are some commonly used escape sequences

Escape Sequence | Meaning | Example | Output
--------------- | ------- | ------- | ------
`\'` | single quote | `print('How\'s Life')` | `How's Life?`
`\"` | single quote | `print("Say \"wow\"")` | `Say "wow"`
`\t` | horizontal tab | `print('aaa\tbbb')` | `aaa` `  ` `bbb`
`\n` | line break | `print('hi\nthere!')` | `hi`<br>`there!`
`\\` | back slash | `print('files\\text')` | `files\text`

You can **use a pair of triple quotes to indicate a multi-line string literal**. 

<tip-box> 

:package: Here is an example multi-line string that uses triple quotes.

<table> 
<tr>
  <td>

```python
print('''Hi,
How's life?
bye!
-me''')
```
  </td>
  <td><br>&nbsp;→&nbsp;</td>
  <td><br>

```
Hi,
How's life?
bye!
-me
```
  </td>
</tr>
</table>

</tip-box>

It is optional to escape `'` and `"` inside a mult-line string within triple quotes e.g., `How's life?` in the example above.

**Triple double-quotes (`"""`) are commonly used to show documentation of code. Such comments are called _docstrings_.**

<tip-box> 

:package: The `remove_head(items)` function below has a docstring that explains its behavior.

```python
def remove_head(items):
  """Removes the first item of the items.
  Expects the list to have at least one item.
  Arguments:
    items (list): the list of items to be modified
  """
  del items[0]
  
numbers = [0, 1]
remove_head(numbers)
print(numbers)
```

</tip-box>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/strings-literals?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>
