## You will start a project today that will be due on Monday at the end of the day. You are going to need to be creative for this project. At this point we have used Tkinter to create the layout of a calculator with buttons, and to create a 3 question quiz. 
### The goal for the next two days is to use Tkinter to create something new. It could be a game, it could be a quiz with some different elements, or it could be something else entirely. You will need to spend some time thinking about what is possible before you start coding. 

### Things we can do right now:
* Create a "label" or text on the screen
* include buttons that call a function when we click on them. (For example command = myClick in the code below calls the function "myClick" that prints 'Hello "name"') 
* We can collect a value from the user that they type in. We can do WHATEVER we can with this variable! Think of all the possibilities...
* We can make buttons certain colors
* We can place buttons in a grid, or wherever we would like
* Additionally, you can always look up (or even ask ChatGPT) how to do particular things, but do not use it for your whole program, or it will not make sense and you won't learn anything. 

```
import tkinter as tk
root = tk.Tk()

e = tk.Entry(root, width=20)
e.pack()

def myClick():
  dontknow = tk.Label(root,text ="I don't know you!")
  myLabel = tk.Label(root, text=("Hello " + e.get()))
  if e.get() == "Jacob":
    myLabel.pack()
  else:
    dontknow.pack()
  

myButton = tk.Button(root, text="Enter your name, then click me", command=myClick)
myButton.pack()

root.mainloop()
```
