# Programming-Lessons
Unit 1 - Intro to elif

### Today we are going to learn how to respond to an answer in more than 2 ways. First, why can't we just use multiple if statements? Let's try that. 

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
