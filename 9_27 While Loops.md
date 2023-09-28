### You're in for a treat! Today we are talking about While loops. We will learn about other loops later, but you will soon discover that loops are a very powerful tool in programming. 

#### So what is a while loop? It is a way to run a program over and over again until a certain condition is met. 
<img src="https://github.com/JTafej/Programming-Lessons/assets/143742710/8bbc0c45-425e-456c-a244-2392c8ae7ef3" width="300" height="300">

#### For example, try running the following code that was demonstrated by our brave volunteer. 

```
counter = 0
while counter < 10:
  print(counter)
  counter +=1
```
#### You will see that the code will run until counter = 10. Amazing. Can you make the program count to 100 instead? 

##### Try running this code. What happens? 
```
exit = ""
while exit = "yes":
  print("🥳")
exit = input("Exit?: ")
```

##### Ah! The "Exit" question was not IN the while loop in that code. See the code below for the correct format for a while loop. 
```
exit = ""
while exit = "yes":
  print("🥳")
  exit = input("Exit?: ")
```

