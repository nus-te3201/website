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

You can specify how to initialize an object of a class by defining an `__init__()` method in the class. 
1. it will be called every time you create an instance of the class.
1. if it has parameters, you need to provide arguments for those parameters when you instantiate an object of that class.

<tip-box> 

:package: 

</tip-box>