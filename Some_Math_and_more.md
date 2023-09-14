# Today we are going to use some math skills in our program. 

### First, I need two volunteers again. 

### Program to reflect what we just did. Try running it in Replit. 
```
myScore = input("Your score: ")
if myScore == 10:
  print("Winner!")
else:
  print("Try again 😭")
```
### We need to tell the program what kind of input we want! In order to do math with an *input*, we must ask for an *integer*! 

We do this by including int() before the input statement. Try the program again. 
```
myScore = int(input("Your score: "))
if myScore == 10:
  print("Winner!")
else:
  print("Try again 😭")
```

### What if we want to include a number that isn't an integer? (ie not 1, 2, 3, 4, 5...) 
### If we want to include a decimal (called a float in python), we simply add float() instead of int()! For example: 

```
myPi = float(input("What is Pi to 2 decimal places? "))
if myPi == 3.14 :
  print("Exactly!")
else:
  print("Try again 😭")
```

