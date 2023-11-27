# Programming-Lessons
Unit 1 - Intro to elif

### From our warmup game, we may have code that looks like this: 
```
flavor = input("What's you favorite flavor of ice cream?")
if flavor == "cookies and cream":
  print("high five!")
else:
  print("Ew!")
```

### What if we wanted to respond to ice cream flavors besides cookies and cream?? Today we are going to learn how to respond to an answer in more than 2 ways. First, why can't we just use multiple if statements? Let's try that. 

#### Run this code and see if you can figure out what the problem is. Tell your neighbor! 
```
age = int(input("How old are you:"))
if age < 21:
  print ("You are a child")
if age >= 21: #Greater than or equal to
  print ("You are an adult")
else:   #Handle all cases where 'age' is negative 
  print ("The age must be a positive integer!")
  
```
##### You'll notice that some issues that occur in coding are hard to see at first. 

<details>
<summary>Answer :) </summary>
<br>
  Try plugging in a number less than 21. You'll notice that the program responds with 2 sentences! That is because it runs both if statements separately.  
  
</details>

### If we want to ask the questions correctly, we must use an elif (else-if) statement. These always go between if statements and else statements. 

#### The correct code will look something like this: 

```
age = int(input("How old are you:"))
if age < 21:
  print ("You are a child")
elif age >= 21: #Greater than or equal to
  print ("You are an adult")
else:   #Handle all cases where 'age' is negative 
  print ("The age must be a positive integer!")
```


### Let's go back to our ice cream example. Let's say we want different actions for different flavors? We will have another demonstration now, and then your job is to write to code to produce this result. First group to have a complete answer on all your computers wins a prize. Comment out your work so it stays in your program when you are done. 

# Now for the challenge of the day. 
## Your task is to create a login system that asks a user for their name, and for their password. Check to see if the username and password match. (You'll need to use AND here.) If the login is successful, print a unique welcome message for each user. (Must have at least 3 unique users.) If another user tries to enter, print red text that says "YOU ARE NOT ALLOWED TO ACCESS THIS PROGRAM," or something like that. 

### To print red text: ###

```
print("\033[31m" "Go away! You do not have an account
here and if you try to log in again, you will be
removed from the server.\033[0m")
```
### Need an extra challenge? Try to use "nesting" to ask multiple if statements for ONE particular user. For example, after they log in successfully, you could ask "How are you feeling today,(name)?" and then provide an appropriate response depending on if they say good, or bad. Example of some nested if statements: 
```
fan = input("So...you are a big rock climbing fan?")
if fan == "yes":
  print("okay cool! But let's just check that")
  style = input("What kind of climbing do you do? TR? Sport? Bouldering...?")
  if style == "Trad":
    print("Okay! A tough guy!")
    protection = input("Do you prefer nuts or cams?")
    if protection == "nuts":
        print("Okay. We're done here. You are awesome.")
    else:
        print("HA! Cams are for the weak.")
  else:
    print("Ha! Pathetic! Trad is the only way to go...")
else:
  print("Thanks for not wasting my time. Goodbye.")
```
### Notice the extra indents after fan == yes. The program is asking more questions if the user says they like rock climbing. Try the program out for yourself. Notice which "else" statements go with which "if" statements. 








