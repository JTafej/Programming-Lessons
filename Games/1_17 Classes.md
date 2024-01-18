## Intro to Classes!
#### In the Space Invaders code we worked with last week, the programmer used something called Classes. We experimented with this code, but it may have been challenging to understand precisely what the code was doing. Today, you will be introduced to the idea of a Class in python. This is a fundamental part of Object-Oriented-Programming. Read more about Object Oriented Programming here: https://www.geeksforgeeks.org/introduction-of-object-oriented-programming/ Note: This is a powerful topic, and gets complicated quickly. We will start with some basics today. 

### Show below is a basic class called "Dog" with attributes name and age. The class also contains two functions (called methods, because they are within the class) that have the dog roll over and sit. This is all our class can do for now. 
```
class Dog:
#A simple attempt to model a dog.
  def __init__(self, name, age):
  #Initialize name and age attributes.
    self.name = name
    self.age = age

  def sit(self):
  #Simulate a dog sitting in repsonse to a command.
    print(f"{self.name} is now sitting.")

  def roll_over(self):
  #Simulate a dog rolling over in response to a command.
    print(f"{self.name} rolled over!")

```



### Your challenge, create a class called Doggy_dice, in which the dog has similar attributes to those shown above, but can also roll a 6 sided die. (You may need to look at previous code to remember how to create a 6 sided die.)


    
