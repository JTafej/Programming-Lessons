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

#### Now that we have learned a bit about these new terms, see if you can fix my code. Run the program a few times to make sure it works properly.

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
<details>
<summary>Hint </summary>
<br>
  Remember: "exit" is a function, so you must include () after it!
  
</details>



#### ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#### ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~





### Your Challenge for today:
#### Your challenge for today is to recreate the Rock, Paper, Scissors game. This time you can use a loop to make the users play multiple rounds! Copy and paste the Rock, Paper, Scissors game below to start with. Your new program should fit the following criteria: 

* Use a loop to repeat the game multiple rounds.
* Keep score of player 1 and player 2.
* End the game when a player wins three rounds using break and exit.
* Use continue to restart the round until one player wins three rounds.
* Your last bit of code should be the results of which player won.
* (There are some hints at the very bottom to help you.) 

```
from getpass import getpass as input

print("E P I C    🪨  📄 ✂️    B A T T L E ")
print()
print("Select your move (R, P or S)")
print()

player1Move = input("Player 1 > ")
print()
player2Move = input("Player 2 > ")
print()

if player1Move=="R":
  if player2Move=="R":
    print("You both picked Rock, draw!")
  elif player2Move=="S":
    print("Player1 smashed Player2's Scissors into dust with their Rock!")
  elif player2Move=="P":
    print("Player1's Rock is smothered by Player2's Paper!")
  else:
    print("Invalid Move Player 2!")
elif player1Move=="P":
  if player2Move=="R":
    print("Player2's Rock is smothered by Player1's Paper!")
  elif player2Move=="S":
    print("Player1's Paper is cut into tiny pieces by Player2's Scissors!")
  elif player2Move=="P":
    print("Two bits of paper flap at each other. Dissapointing. Draw.")
  else:
    print("Invalid Move Player 2!")
elif player1Move=="S":
  if player2Move=="R":
    print("Player 2's Rock makes metal-dust out of Player1's Scissors")
  elif player2Move=="S":
    print("Ka-Shing! Scissors bounce off each other like a dodgy sword fight! Draw.")
  elif player2Move=="P":
    print("Player1's Scissors make confetti out of Player2's paper!")
  else:
    print("Invalid Move Player 2!")
else:
  print("Invalid Move Player 1!")
```
# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Hints:
* Create a counting system using a variable and += to keep track of the winner for each round.
* The while loop needs to be at the start of the game.
* Make sure you include print statements saying each player's final score at the end.
* Create an if statement to end the loop.

