---
title: Number Guessing Game
difficulty: intermediate
languages: all
estimate: '2 hours'
---

Practice your loops and conditionals by creating an interactive number guessing game.

### Project Description
For this activity, you will write a program in your language of choice that
will play a Guess the Number Game with you.

This program will randomly generate an integer between 0 and 99 (inclusive,
meaning 0 and 99 are possible choices) and will then keep asking the user to
guess what that number was.

If the user has guessed an incorrect number, the program should respond with
either "Too High" or "Too Low", depending on which is true.

If the user has guessed the correct number, the program will end, and tell the
user how many guesses it took the human to get it right. In addition, there
should be a message based on that number:

* **1 guess:** That was lucky!
* **2-5 guesses:** Good Job.
* **6 or more guesses:** Not very impressive.

It is okay to mess around with these messages, but try to get the program
working first!

### Sample Output
A working version of this program might look similar to this when it runs:
```
Enter a guess between 1 and 99: 35
Too High!

Enter a guess between 1 and 99: 15
Too High!

Enter a guess between 1 and 99: 10
Too High!

Enter a guess between 1 and 99: 5
Too Low!

Enter a guess between 1 and 99: 7
Too Low!

Enter a guess between 1 and 99: 8
Yeah! Your guess was correct.

I had chosen 8 as the target number.
You guessed it in 6 tries.
Not impressive.
```

### Follow-up
* Have you considered the most efficient way to play? What should always be
  your starting guess?
  * What are always your possible 2nd guesses?
  * This kind of thing is called a **Binary Search**, where we always reduce the search space by 1/2 (or close to that)
* Can you try to make a new version of this program where both players are computers?
  * See if you can't make the computer always solve this problem *optimally* using the strategy above.
  * You will have to keep track of at least three variables, like `minimumPossibleGuess`, `maximumPossibleGuess`, and the halfway point between them: `guess`
