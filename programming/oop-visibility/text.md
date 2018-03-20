### Visibility

The _encapsulation_ aspect of OOP requires that an object should only allow controlled access to its members. For example, it should be able to make some of its attributes visible to other object while keeping others hidden. As a consequence of Python's aim to be a very flexible and versatile language, it does not enforce encapsulation as strictly as some other OOP languages. However, it recommends some conventions, if followed, will maintain a reasonable level of encapsulation in objects.

* **_Private_ members: An attribute/method whose name has at least two leading underscores and at most one trailing underscore (e.g., `__foo`, `__bar_()`) cannot be accessed using its name by code outside the class.** These are 

* **_Protected_ members: a name prefixed with a single underscore (e.g. `_foo`, `_bar()`) are -- by convention -- should not be accessed by code outside of the owner class** as they are not meant to be part of the object's public interface.

* **_Public_ members: other members are considered public and OK to be accessed by code outside the class.**

<tip-box> 

:package: Consider the `Account` class below.

```python
class Account:
  currency = '$'   # public
  _min = 10.       # protected
  __max = 1000.0   # private
  
  def __init__(self, person, amount):
    self.__balance = amount # private
    self._owner = person    # protected
    self.status = 'OK'      # public
    
  def get_info(self):       # public
    return [self.status]
    
  def get_loan_limit(self): # public
    return self.__get_income()*5
    
  def _get_more_info(self): # protected
    return self.get_info() + [self._owner]
    
  def __get_income(self):   # private
    return self.__balance + 100
```
:white_check_mark: The following code works fine because the members being accessed are public.
<table> 
<tr>
  <td>

```python
print('currency:', Account.currency)
a = Account('Adam', 100)
print('status:', a.status)
print('info:', a.get_info())
```
  </td>
  <td valign="bottom">&nbsp;→&nbsp;<br><br></td>
  <td valign="bottom">

```
currency: $
status: OK
info: ['OK']
```
  </td>
</tr>
</table>

:exclamation: The following code works too. But they access protected members which is ==not a recommended practice==.
<table> 
<tr>
  <td>

```python
print('minimum allowed:', Account._min) 
a = Account('Adam', 100)
print('owner:', a._owner) 
print('more info:', a._get_more_info())
```
  </td>
  <td valign="bottom">&nbsp;→&nbsp;<br><br></td>
  <td valign="bottom">

```
minimum allowed: 10.0
owner: Adam
more info: ['OK', 'Adam']
```
  </td>
</tr>
</table>

:x: The following code will not work because they try to access private members.
<table> 
<tr>
  <td>

```python
print('maximum allowed:', Account.__max) # error
a = Account('Adam', 100)
print('balance:', a.__balance) # error
print('income:', a.__get_income()) # error
```
  </td>
  <td valign="bottom">&nbsp;→&nbsp;<br><br></td>
  <td valign="bottom">

```
AttributeError: type object 'Account' has no attribute '__max'...
AttributeError: 'Account' object has no attribute '__balance'...
AttributeError: 'Account' object has no attribute '__get_income'...
```
  </td>
</tr>
</table>

:bulb: Although this example does not have class-level methods, note that the same visibility conventions apply to them as well.
</tip-box>

<panel type="danger" header=":muscle: Exercise: Change Visibility of `School` Class Members" expanded no-close>
  <include src="e-changeVisibilityOfSchoolClassMembers.md" />
</panel><p/>