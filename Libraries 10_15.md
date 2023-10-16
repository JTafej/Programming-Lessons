## Today we are going to talk about a very important thing called Libaries. 

### There currently around 137,000 python libriaries. Holy Cow! Here is a link to the 10 most popular libraries. Take a minute to read through each one and learn what they are used for. 
#### https://www.geeksforgeeks.org/libraries-in-python/

### For example, PyTorch is used for Machine learning and Neural Networks. 
* "PyTorch is the largest machine learning library that optimizes tensor computations. It has rich APIs to perform tensor computations with strong GPU acceleration. It also helps to solve application issues related to neural networks."

### How do you use a library? It's not too complicated! You just have to "import" the library, and then call the function or module you want to use from the library. For example:
#### This program will use the function randint from random to select a random integer between 1 and 100!
```
import random
myNumber = random.randint(1,100)
print(myNumber)
```
#### Try this one (There are a couple of errors you'll need to fix first.) Make sure to comment this in your program. Call me over when you are done so I check you off. 
```
import random
for i in range(10):
  myNumber = randint(1, 100)
  print(Number)
```

### Okay, that's pretty cool. But we can do much more with Libraries!
#### For example, we can use the os library to talk directly to the console! 

```
import os
for i in range(1,1000):
  print(i)
```
### Hmm... Okay, not much going on here yet. We imported os, but we actually have to use it! Check it out:
```
import os
for i in range(1,1000):
  print(i)
  os.system("clear")
```
### Amazing! This is a very powerful tool, as it can clear our results and make the program a lot more pleasant for the user. 
#### What is the problem here?
```
import os
adding = 4 + 3
print(adding)
os.system("clear")

subtraction = 8 - 9
print(subtraction)
os.system("clear")

multiplication = 4 * 32
print(multiplication)
os.system("clear")

division = 50 / 5
print(division)
os.system("clear")

squared = 5**2
print(squared)
os.system("clear")
```
### Well, the program is doing the calculations, but they are getting deleted instantly! If we use the "time" library, we can see the answers just for a minute!
```
import os, time
adding = 4 + 3
print(adding)
time.sleep(1)
os.system("clear")

subtraction = 8 - 9
print(subtraction)
time.sleep(1)
os.system("clear")

multiplication = 4 * 32
print(multiplication)
time.sleep(1)
os.system("clear")

division = 50 / 5
print(division)
time.sleep(1)
os.system("clear")

squared = 5**2
print(squared)
time.sleep(1)
os.system("clear")
```

### Okay, now it's time for the challenge of the day. 
