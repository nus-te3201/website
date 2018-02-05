#### Exercise : Word Game

Implement a word game with the following rules:
* The player inputs four-letter words. Words that are not four letters are rejected.
* If the player inputs the same word multiple times, that word is _banned_.
* When the player cannot think of any more suitable words, he/she can end the game by entering the word `end`
* The score is the number of words entered by the player and accepted by the game (i.e., banned words are not counted)
 
Given below is a sample session. Try to follow the exact output format in your implementation:
```
========================================================
Welcome to the WORD GAME
Give all four-letter words you know, one word at a time
Enter the word e to exit
========================================================
What's the next word?  part
What's the next word?  puck
What's the next word?  cut
Not a four-letter word
What's the next word?  part
Repeated word! part is number  1 in the accepted words list.
part is no longer an accepted word and is banned
What's the next word?  bust
What's the next word?  team
What's the next word?  puck
Repeated word! puck is number  1 in the accepted words list.
puck is no longer an accepted word and is banned
What's the next word?  puck
puck is banned!
What's the next word?  read
What's the next word?  meat
What's the next word?  read
Repeated word! read is number  3 in the accepted words list.
read is no longer an accepted word and is banned
What's the next word?  end
========================================================
Your score: 3
Accepted words (in order of entry): bust team meat
Accepted words (in sorted order): bust meat team
Banned words (in sorted order): part puck read
Thank you for playing the WORD GAME
========================================================
```

:bulb: Implementation suggestions:
* Maintain two lists: one to keep accepted words, one to keep banned words
* When a word is entered for the second time, move it from the _accepted words_ list to the _banned words_ list. 
