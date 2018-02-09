### Object References

**Objects of some Python _types_ are _immutable_.** An immutable object, once created, cannot be modified.

Some immutable types:

* int
* float
* decimal
* complex
* bool
* string
* tuple
* range
* frozenset
* bytes

**Objects of some other Python types are _mutable_.** A mutable object can be modified during its lifetime.

* list
* dict
* set
* bytearray

**An _object reference_ is simply the address of the memory where an object is currently stored.**

<tip-box> 

:package: In the example below, the variable `spam` is pointing to the list object `[0, 1, 2, 3, 4, 5]` by way of storing the reference to the list object.

`spam = [0, 1, 2, 3, 4, 5]`<br>
![](https://automatetheboringstuff.com/images/000081.jpg)<br>
<sub>Image credit: [AtBSwP](https://automatetheboringstuff.com)</sub>

</tip-box>

**When you assign variables as  `v1 = v2`, if `v2` is pointing to an immutable object, a copy of the object is assigned to `v1`.**
However, **if `v2` is pointing to a mutable object, its object reference (not the object itself) is copied to `v1`** so that now both `v1` and `v2` are pointing to the same object.