#### Exercise : Vending Machine - Add Loop

The code below simulates a vending machine that asks for a coin and gives out the product and the balance.
```python
price = 100
coin_value = 0

print('Price:', price)

coin_value = int(input('Enter a coin:'))
print('You have entered:', coin_value)

print('Here is the product')
print('Your balance:', coin_value - price)
```
:bulb: When you give a string argument to the `input` function e.g., `input('Enter a coin:')`, it shows the string to the user and reads the input from the user.

Example output from the code:
```python
Price: 100
Enter a coin: 200
You have entered: 200
Here is the product
Your balance: 100
```

As you can see, this code does not consider the case where the inserted coin is less than the price of the product, resulting in the following incorrect behavior.

```python
Price: 100
Enter a coin: 50
You have entered: 50
Here is the product
Your balance: -50
```

Modify the code to repeat these two lines until the coin entered is enough to pay for the product.
```python
coin_value = int(input('Enter a coin:'))
print('You have entered:', coin_value)
```

The output should be something like this:
```python
Price: 100
Enter a coin: 50
You have entered: 50
Enter a coin: 100
You have entered: 100
Here is the product
Your balance: 0
```