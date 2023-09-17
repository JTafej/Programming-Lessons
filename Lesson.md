### First thing today we are going to run through this code and decide what the program is doing. Afterwards, you will alter the code. 

```
print("POSITIVITY MACHINE!!", "\n",
      "++++++++++++++++++++++++++","\n")
name = input("Glad you're using this machine. So, what's your name?")
if name == "Jacob" or name == "jacob":
  print("Hey Jacob. What are you hoping to get done with your life today? Think small. Just today.")
  task = input("List one simple task here.")
  rating = input("Great. I beleive in you! Maybe you could tell me more about how your day has been so far. Give me 1-5 rating!")

  if rating == "1":
    print("ahh dang. Well, despite that, I am sure you will be able to" , task, " \n I bet your day will improve, whether or not you complete that task")
  elif rating == "2":
    print("Okay! Better than a 1 right?? I am sure you will be able to" , task,  "\n And I bet your day will improve :)")
  else:
    print("Booya! That's not bad! I am sure you will complete", task, "and then your day will be even better!")

else :
  print("Ah, I don't know you", name, "so I don't think I can help you any further. \n However, I hope you have an amazing day :)")
```
#### Last class we talked about integers and floats. Remind your neighbor why it is sometimes useful to use numbers in your code. 

<details>
<summary>Reminder </summary>
<br>
  Numbers can be useful when we want to compare values. For instance, if I want to find out if someone scored less that 70% on the test, I would need to use an integer. Ex. (56 <= 70) 
  
</details>

##### Run the following to remind yourself how integers work in python. (Notice "int" next to input. This is telling the program that the user is entering an integer. This is called *casting.* Try plugging in a word instead and see what happens!)  

```
myScore = int(input("Your score: "))
if myScore >= 70:
  print("Nice job!")
else:
  print("Better luck next time...")
```







