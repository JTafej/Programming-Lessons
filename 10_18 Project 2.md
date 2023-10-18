## Happy Wednesday. Today, we are going to start project 2!

### Before we get into it, we do have a bit of new material to cover: 

### Subroutines! Subroutines are like recipes. Below is an example of a subroutine that rolls a 6 sided die. 
```
def rollDice():
  import random
  dice = random.randint(1, 6)
  print(dice)

rollDice()
```
### Practice this one. You'll that rolls a 6 sided die. This "subroutine" will run each time it is told to do so. For example, try this: 
```
def rollDice():
  import random
  dice = random.randint(1, 6)
  print(dice)

rollDice()
rollDice()
rollDice()
```

### Okay, that's cool. But we can't really do anything with the results of this subroutine, as it currently exists. What if we want to have a specific reply based on the roll?
### We must add "return." Example below: 

```
def rollDice():
  import random
  dice = random.randint(1, 6)
  print(dice)
  return dice
roll = rollDice()
```
### Now you have a variable called "roll" that is equal to the value of that particular roll. You can use that variable to give a specific response, like the following: 

```
def rollDice():
  import random
  dice = random.randint(1, 6)
  print(dice)
  return dice
roll = rollDice()
if roll < 5:
  print("Ahh you got eaten by a big bear!")
else:
  print("You survived!")
```
## Your job for project 2 is to create a role playing game that involves loops and rolling dice. Use the code above for inspiration. Look through all past assignments and your last project for inspiration. Use os.system("clear") to make your console look simple. You have learned a fair amount now, and can make a pretty fun adventure game. Due at the end of the day on Monday, 10/23










