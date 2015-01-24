# input1.py Walkthrough

Annotated Source:
```python
import random              # Import the random module from python

x = random.randrange(100)  # Assign x a random value from 0 to 100

y = input()                # Get input from the user and evaluate it
                           # Assign the evaluated value to y

while x != y:              # While x is not the same value as y continue to execute the indented commands
    print "Nuh uh"         # Print "Nuh uh" to the user
    y = input()            # Get input from the user and evaluate it
                           # Assign the evaluated value to y

print "YOU DID IT :D"      # Print "Nuh uh" to the user

```

This is a pretty staight forward program, get a random value and while the value the user enters is not equal to the random value, "Nuh uh", will be printed back to the user.

So the obvious approach to getting "YOU DID IT :D" to appear is to just guess the numbers 0 to 100 and eventually one of the values will be right, but what if the range of randomness was expaned to 100,000 or everytime the `while` loop was executed x was assigned another random value `x = random.randrange(100)`. Our approach would no longer work so let's come up with something that works 100% of the time on the first guess.

So if we look up the [python documentation](https://docs.python.org/2/library/functions.html#input) for `input()` we see that it syntactically the same as `eval(raw_input())` and from what we know about `raw_input()` we know it grabs input from the user and `eval(statement)` will evaluate `statement` as a python command. Hmmm. Well if we open up an interpreter and type:

```python
>>> import random
>>> x = random.randrange(100)
>>> x
12
```
So `x` by itself is a valid python expression so what if we type `x` instead of a number when the program asks for our input? Effectively, instead of `y = input()` our program would conceptually become `y = x` and since the `while` loop only continues when `x != y`, the `while` loop will stop and we will get the nice little message showing us that we completed the challenge :D

