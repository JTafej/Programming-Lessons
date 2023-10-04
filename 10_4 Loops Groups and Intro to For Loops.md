## Hello! Today we are going to do another coding Relay! 
#### These are the groups: 
* Group 1: James, TA, Max
* Group 2: Hank, Kevin, Rory
* Group 3: Taixi, Reiko, Paddy

### Your Relay challenge is as follows: 
#### Create a Guess-the-number Game using a while True loop. It should include the following elements: 
* First print something like "Can you guess the number? Your odds are one in a million!"
* You should choose the magic number between 1-1,000,000
  * Basically, YOU create a variable for the magic number. 
* The program should include a while True loop
* If the guess is too high, say "Too high!" If the guess is too low, say "too low!"
  * You will need to use IF statements here in order to compare the users input to the magic number. 
* The program should continue to ask the user to a guess until they get it correct.
  * After the guess correctly, the loop should end! How do you do this? 
* Lastly, include a counter that will tell the user how many tries it took them to guess. 

> USE PAPER AND PENCIL TO MAP OUT A PROGRAM! WORK AS A TEAM SO YOU KNOW WHAT YOU SHOULD BE WRITING EACH TIME YOU GO TO THE COMPUTER 


## 
## 


### Now, for something new. We are going to learn a different type of loop! (This is to be completed in the "For Loops Intro" Replit.)
#### "For Loops" Provide a way to run a loop an exact number of times. While loops would run until we met a certain condition. For loops are used when we know how many times we want them to be run. 

#### For example, take this while loops we saw last week: 
```
counter = 0
while counter < 10:
  print(counter)
  counter += 1
```
#### We can instead right this as a for loop, because we know we want to count up to 10. 
```
for counter in range(10):
  print(counter)

```
#### Another For Loop example: 

```
for x in range(6):
  if x == 3: break
  print(x)
else:
  print("Finally finished!")
```

#### notice the new term "range." range counts from 0-9, and in this case will print numbers 0-1. Range is a function, like exit, so we must include paranthesis after. example: range(4)
#### In the loop above "counter" is the variable. "i", "j", and "k" are commonly used by programmers as variables in for loops. 


