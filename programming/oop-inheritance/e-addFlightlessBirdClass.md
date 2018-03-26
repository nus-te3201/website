#### Exercise : Add `FlightlessBird` Class

Do the following changes to the given code so that the code below produces the given output:
1. update the `info()` method of the `Bird` to call the same method from the parent class
1. add a `FlightlessBird` class that inherits from the `Bird` class, and override the `move()` method 

<table>
<tr>
  <td>

```python
class Animal:

  def __init__(self, name):
    self.name = name
    
  def info(self):
    print("I'm a", self.name)
    

class Bird(Animal):

  def move(self):
    print("I'm flying")
    
  def info(self):
    # CALL info() METHOD OF PARENT CLASS HERE 
    print("I have feathers")

# ADD FlightlessBird CLASS HERE

crow = Bird('Crow')
crow.info()
crow.move()
penguin = FlightlessBird('Penguin')
penguin.info()
penguin.move()
```
  </td>
  <td valign="bottom">&nbsp;→&nbsp;<br><br></td>
  <td valign="bottom"> 

```
I'm a Crow
I have feathers
I'm flying
I'm a Penguin
I have feathers
I'm waddling
```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:bulb: Partial solution%%">

```python
class FlightlessBird(Bird):

  def move(self):
    ...
```

</panel>