### Visibility

The _encapsulation_ aspect of OOP requires that an object should only allow controlled access to its members. For example, it should be able to make some of its attributes visible to other object while keeping others hidden. As a consequence of Python's aim to be a very flexible and versatile language, it does not enforce encapsulation as strictly as some other OOP languages. However, it recommends some conventions, if followed, will maintain a reasonable level of encapsulation in objects.

**_Private_ members: An attribute/method whose name has at least two leading underscores and at most one trailing underscore (e.g., `__foo`, `__bar_()`) cannot be accessed using its name by code outside the class.** These are 

**_Protected members: a name prefixed with a single underscore (e.g. `_foo`, `_bar()`) are -- by convention -- should not be accessed by code outside of the owner class** as they are not meant to be part of the object's public interface.