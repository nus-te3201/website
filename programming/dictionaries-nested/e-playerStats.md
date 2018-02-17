#### Exercise: Player Stats

Note how the `player_stats` dictionary in the code below uses nested dictionaries to store, for each player, how many times the player scored a certain hit size (which can be 0, 1, 4, 6). For example, `'amy': {0:0, 1:2, 4:0, 6:1}` means player `amy` scored hit size of 0 x 0 times; hit size of 1 x 2 times; hit size of 4 x 0 times; hit size of 6 x 1 time.

Update the `get_player_hit_count(player_stats, player, hit_size)` functions in the code such that it uses the `player_stats` dictionary to return the hit count for the `player` for the given `hit_size`.


```python
player_stats = {'amy': {0:0, 1:2, 4:0, 6:1},
          'betty': {0:2, 1:0, 4:2, 6:0},
          'charlie': {0:0, 1:0, 4:0, 6:4}}
          
def get_player_hit_count(player_stats, player, hit_size):
  return 0 #REPLACE WITH YOUR CODE!

print(get_player_hit_count(player_stats, 'amy', 4))
print(get_player_hit_count(player_stats, 'betty', 0))
```
:arrow_heading_down:
```
0
2
```

<panel type="seamless" header="%%:bulb: Partial solution%%">

```python

def get_player_hit_count(player_stats, player, hit_size):
  return player_stats[...][...]
```

</panel>