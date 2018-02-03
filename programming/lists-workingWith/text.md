### Working with Lists

**You can use the `len` function to find the number of items in a list.**

<tip-box> 

<table>
<tr>
  <td>
  
```python
spam = ['a','b']
print('Length is:', len(spam))
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```

Length is: 2

```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-len-plus-star-for?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>

</tip-box>

**You can use the `+` operator to combine two lists into a new list.**

<tip-box> 

<table>
<tr>
  <td>
  
```python
girls = ['Amy', 'Betsy', 'Clara']
boys = ['Adam', 'Ben']
friends = girls + boys
print(friends)
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```



['Amy', 'Betsy', 'Clara', 'Adam', 'Ben']

```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-len-plus-star-for?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>

</tip-box>

**You can use the `*` operator to create a new list by replicating an existing list multiple times.**

<tip-box> 

<table>
<tr>
  <td>
  
```python
steps = ['left', 'right']
walking = steps*3
print(walking)
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```


['left', 'right', 'left', 'right', 'left', 'right']

```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-len-plus-star-for?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>

</tip-box>

<panel type="seamless" header="%%:tv: Length of a list, list concatenation, list replication%%">
<iframe width="560" height="315" src="https://www.youtube.com/embed/5n6o1MaXDoE?rel=0&showinfo=0&start=581&end=635&version=11" frameborder="0" allowfullscreen></iframe>

</panel><p/>

**You can use `in` or `not in` to check if an item is in a list**. 

<tip-box> 


```python
valid_responses = ['Yes', 'No', 'Maybe']
response = ''
while response not in valid_responses:
  response = input('What is your response?')
print('Your response:', response)

current_drinks = ['Tea', 'Coffee']
suggested_drink = input('Suggest a new drink:')
if suggested_drink in current_drinks:
  print(suggested_drink, 'is already in the list')
```
:arrow_heading_down:
```
What is your response? abc
What is your response? Yes
Your response: Yes
Suggest a new drink: Tea
Tea is already in the list
```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-in-not-in?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>

</tip-box>

<panel type="seamless" header="%%:tv: Checking if an item is in a list%%">
<iframe width="560" height="315" src="https://www.youtube.com/embed/5n6o1MaXDoE?rel=0&showinfo=0&start=675&end=742&version=11" frameborder="0" allowfullscreen></iframe>

</panel><p/>

**You can traverse through items in a list using the `for item_name in list_name:` notation**.

<tip-box> 

<table>
<tr>
  <td>
  
```python
pets = ['Cats', 'Dogs', 'Hamsters']
for animal in pets:
  print('Do you sell '+ animal +'?')
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```

Do you sell Cats?
Do you sell Dogs?
Do you sell Hamsters?
```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-len-plus-star-for?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>

</tip-box>

**The `enumerate` function can help you easily maintain an iteration counter while traversing a list**.

<tip-box> 

<table>
<tr>
  <td>
  
```python
pets = ['Cats', 'Dogs', 'Hamsters']
for i, animal in enumerate(pets):
  print(i+1, 'Can I buy '+ animal +'?')
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```

1 Can I buy Cats?
2 Can I buy Dogs?
3 Can I buy Hamsters?
```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/lists-len-plus-star-for?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel>

</tip-box>