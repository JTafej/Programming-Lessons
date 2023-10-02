## Welcome Back! Today we are going to continue using While Loops. We are going to learn a few new commands as well. 

#### Here is the code I was running at the start of class. Mess around with it to learn more about how exit, break, and continue work for while True
```
while True:
  print("You are in a corridor, do you go left or right?")
  direction = input("> ")
  if direction == "left":
    print("You have fallen to your death")
    break
  elif direction == "right":
    continue
  else:
    print("Ahh! You're a genius, you've won")
    exit()
print("The game is over, you've failed!")
```

#### Now that we have learned a bit about these new terms, see if you can fix my code: 

```
print("Let's play chutes and ladders. Pick ladder or chute.")
while True:
  print("Do you want to go up the ladder or down the chute?")
  direction = input("> ")
  if direction == "chute"
    print("Game over!")
  break
  elif direction == "ladder":
    continue
else:
    print("Game over!")
    exit 
print("Thanks for playing!")
```







