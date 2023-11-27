### Today's lesson will involve using For Loops in more ways. We will also expand on the Range() function. 


#### First of all, Range can do more than just tell us a list of numbers (Remember range(10) is 0-9) 

#### As it turns out, range can take more than just one input! For example, the following code will print the numbers 100-109. Try it for yourself. 
```
for i in range(100, 110):
  print(i)
```
#### Now try this code. Notice we have a concatenated print statement in the for loop! Pretty cool. 
```
for i in range(1, 8):
  print("Day", i)
````
#### Put it to use! 
```
print("Thirteen Times Table")
for i in range(1, 13):
  print(i, "x 13 =", i * 13)
```

#### Okay, now we are going to add a THIRD input to range. This third input will tell the user what INCREMENT to count by. For example, the following code will count from 0 to 1000000 by 25. Try it. 

```
for i in range (0, 1000000, 25):
  print(i)
```

#### You can actually put a variable INTO the range function. For example: 
x = 2
y = 6
for i in range(x, y):
  print(i)

### Your challenge for today: Ask the user what numbers they want to print (starting value and ending value) and then ask them what they want to increment by. After that, run a for loop with the user's input. For an extra challenge, can you create a program that generates the time's table of the users choice? 






