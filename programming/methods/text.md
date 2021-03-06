### Methods

**In Python, everything is an object.** For example, `'Hello'` (is a string object),  `14` is an integer object, `[2.0, 3.5]` is a list object that contains two float objects, and so on.

Accordingly, **most Python objects have _methods_**. Methods represent what the object can do. They are functions attached to an object and are executed in relation to the attached object. Methods are executed using `object.method_name` notation. The methods an object will have depend on the _type_ of object %%&nbsp;e.g., methods a string object will have are different from the methods a list object will have%%.

<tip-box> 

:package: The first line below uses the `strip()` method of the string object to get rid of leading and trailing spaces. The second statement uses the `replace()` method to replace spaces with dashes. 

<table> 
<tr>
  <td>

```python
print('[' + '  some text  '.strip() + ']')
print('some simple words'.replace(' ', '-'))
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>

```

[some text]
some-simple-words
```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/methods?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>

</tip-box>

Some methods return an object. In such cases another method can be called on the returned object immediately. Such **calling of methods on the returned object is called _method chaining_.**

<tip-box> 

:package: In the example of method chaining given below, `'aa bb cc  '.strip()` returns a string object `'aa bb cc'` on which the `replace(' ', '_')` method is called. That returns a string object `'aa_bb_cc'` on which the `upper()` method is called. That method converts the string into its upper case, giving us the final output of `'AA_BB_CC'` 

<table> 
<tr>
  <td>

```python
print('aa bb cc  '.strip().replace(' ', '_').upper())
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>

```

AA_BB_CC
```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/methods?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>

</tip-box>

<panel type="danger" header=":muscle: Exercise: Remove Extra Spaces" expanded no-close>
  <include src="e-removeExtraSpaces.md" />
</panel><p/>

 

