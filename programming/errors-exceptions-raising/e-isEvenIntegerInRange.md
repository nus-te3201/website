#### Exercise : Is Even-Integer in Range

Complete the functions in the code below to behave as follows:
* `confirm_is_int(number)`: Raises a `ValueError` if the `number` is not an integer.<br>
  :bulb: You can use the `type(value) is type_name` and `type(value) is not type_name` to check if a `value` is of type `type_name`<br>e.g., `type('x') is not float` evaluates to `True` because `'x'` is not a `float`. [[more examples ...](https://www.poftut.com/python-type-function-examples/)]
* `confirm_range_correct(start, end)`: Raises a `ValueError` if `end` or `start` are not integers or if `start` is greater than `end`.

These functions have been implemented fully. Their behavior:
* `is_even_int(number)`: Returns `True` if the `number` is an even integer. Raises a `ValueError` if the `number` is not an integer.
* `is_in_range(number, start, end)`: Returns `True` if the `number` is in the range `start` to `end` (==including `start` but excluding `end`==, as per how Python define _ranges_). Raises a `ValueError` if if the `number` is not an integer or `start` and `end` do not specify a range correctly.
* `is_even_int_in_range(number, start, end)`: Returns `'Yes'` if `number` is an even integer in the range `start` to `end`. Returns `'No'` otherwise. Returns an error message if any of the inputs are incorrect. The example output given below has the output of the error message. 

```python
def confirm_is_int(number):
  pass # ADD YOUR CODE HERE!


def confirm_range_correct(start, end):
  confirm_is_int(start)
  confirm_is_int(end)
  # ADD YOUR CODE HERE!

  
def is_even_int(number):
  confirm_is_int(number)
  return int(number)%2 == 0


def is_in_range(number, start, end):
  confirm_is_int(number)
  confirm_range_correct(start, end)
  return number >= start and number < end


def is_even_int_in_range(number, start, end):
  try:
    if is_even_int(number) and is_in_range(number, start, end):
      return 'Yes'
    else:
      return 'No'
  except ValueError as e:
    return 'Value error: ' + str(e)


def is_even_int_in_range(number, start, end):
  try:
    if is_even_int(number) and is_in_range(number, start, end):
      return 'Yes'
    else:
      return 'No'
  except ValueError as e:
    return 'Value error: ' + str(e)

def check(number, start, end):
  print(number, 'is an int in range', start, '-', end, '?', is_even_int_in_range(number, start, end))


# some examples of using is_even_int_in_range
check('x', 'y', 'z')
check(3, 'y', 'z') # False (3 is not even)
check(2, 3.4, 5)
check(2, 3, [])
check(2, 5, 1)
check(2, 5, 5)
check(3, 1, 5)
check(4, 1, 4) # False ( range 1 to 4 excludes 4)
check(4, 1, 5)
```
:arrow_heading_down:
```
x is an int in range y - z ? Value error: x is not an integer
3 is an int in range y - z ? No
2 is an int in range 3.4 - 5 ? Value error: 3.4 is not an integer
2 is an int in range 3 - [] ? Value error: [] is not an integer
2 is an int in range 5 - 1 ? Value error: start is smaller than end
2 is an int in range 5 - 5 ? No
3 is an int in range 1 - 5 ? No
4 is an int in range 1 - 4 ? No
4 is an int in range 1 - 5 ? Yes
```

<panel type="seamless" header="%%:bulb: Partial solution%%">

```python
def confirm_is_int(number):
  if type(number) is not int:
    raise ValueError(str(number) + ' is not an integer')
```

</panel>