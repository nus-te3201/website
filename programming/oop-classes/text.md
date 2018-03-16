### Classes

As you have seen already, Python has some built in object types (i.e., classes) such as `list`, `int`, `str`, etc. In addition, **you can define your own classes** in Python.

The syntax for defining a class:
```python
class ClassName:
  # method definitions
```
:bulb: It is customary to use <trigger trigger="click" for="modal:classes-camelcase">Upper Camel Case</trigger> for class names.

The syntax for **creating (also called _instantiating_) an object** of the class is `ClassName()`.

<modal title="CamelCase" id="modal:classes-camelcase">

![](https://upload.wikimedia.org/wikipedia/commons/e/ef/CamelCase.svg =200x)<br>

Camel Case refers to a styling text writing compound words or phrases such that each word or abbreviation in the middle of the phrase begins with a capital letter, with no intervening spaces or punctuation e.g., `freshAppleJuice`. _Upper Camel Case_ (also called _Pascal Case_) is similar to Camel Case except the first letter is capitalized as well e.g., `FreshAppleJuice`.

<sub>[source: [Wikipedia](https://en.wikipedia.org/wiki/Camel_case)]</sub>
</modal>

<tip-box> 

:package: The code below defines a class named `Employee`, creates two employee objects, and prints the class/type of each object.

```python
class Employee:
  pass # an empty class

john = Employee() # create an Employee object
print(type(john)) # print type of the john object
alice = Employee()
print(type(alice))
```
:arrow_heading_down: %%Note how the type of each object is given as `class Employee`.%%
```
<class 'Employee'>
<class 'Employee'>
```
</tip-box>

You can add methods to the class by defining them inside the class definition. Note that a method of a class always take `self` as the first parameter. `self` refers to the object itself. When calling the method, there is no need to supply an argument for the `self` parameter as the target object is implicitly taken as the argument for that parameter.

<tip-box> 

:package: In the example below, `write(self, text)` method is called as `p.write('It was a dark night ...')`. This is how the arguments are matched with the parameters: 
* `self` → `p`
* `text` → `'It was a dark night ...'`

<table> 
<tr>
  <td>

```python
class Pen:
  
  def write(self, text):
    print('writing:', text)
    
p = Pen()
p.write('It was a dark night ...')
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>

```
writing: It was a dark night ...
```
  </td>
</tr>
</table>

</tip-box>

**You can specify how to initialize an object of a class by defining an `__init__()` method in the class.** Here are the important things to note about the `__init__()` method: 
1. There are two underscores in front and two behind the word `init`.
1. Tt will be called every time you create an instance of the class.
1. If it has parameters, you need to provide arguments for those parameters when you instantiate an object of that class.

<tip-box> 

:package: 

```python
class Person:
  
  def __init__(self, name):
    print('Person object', name, 'initialized!')
    
tom = Person('Tom')
```
:arrow_heading_down:
```
Person object Tom initialized!
```
</tip-box>

The code within a class needs to use the `self.` to refer to its own attributes and methods. Furthermore, the best place to initialize attributes is the `__init__()` method.

<tip-box> 

:package: Note how the `__init__()` method of the `Book` class initializes its two attributes and calls another of its own methods i.e., `self.describe()`.

```python
class Book:
  
  def __init__(self, book_title, book_author):
    self.title = book_title # initialize attribute title
    self.author = book_author # initialize attribute author
    self.describe() # call another method of the class
    
  def describe(self):
    print('Book info:', self.title, '/by', self.author) # use attributes of the class
    
b = Book('The Jungle Book', 'Leo Tolstoy')
b = Book('The Art of War', 'Sun Tzu')
```
:arrow_heading_down:
```
Book info: The Jungle Book /by Leo Tolstoy
Book info: The Art of War /by Sun Tzu
```
</tip-box>