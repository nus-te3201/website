#### Exercise: Detailed Scores

Update the `get_detailed_scores` functions in the code such that it stores a ==list of integers for each player==, instead of one integer for each player, so that we can use the dictionary to store different scores each palyer scored in multiple innings of the game.

Player | Scores in different innings
-------|---------------------------
amy    | 5, 5, 10
betty  | 10, 10, 10
charile| 5, 10, 15

```python
def get_detailed_scores():
  return {'amy': 20, 'betty': 30, 'charlie': 30} #REPLACE WITH YOUR CODE! 

print(get_detailed_scores())
```
:arrow_heading_down:
```
{'amy': [5, 5, 10], 'betty': [10, 10, 10], 'charlie': [5, 10, 15]}
```

<panel type="seamless" header="%%:bulb: Partial solution%%">

```python
def get_detailed_scores():
  return {'amy': [5, 5, 10],
          ...}
```

</panel>