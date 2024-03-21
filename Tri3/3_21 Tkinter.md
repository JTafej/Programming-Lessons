## Hello everyone! Today we will start with a group project, and then you will have some time to work individually on projects. 

### The group project is to use tkinter to create a F to C and C to F temperature converter. You need to have two different buttons, one should convert from F to C, and the other should convert from C to F. Do this in a group of two or three, and make sure each of you have access to the replit. Use the code below as a tempplate to start with. 
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

### After your group has submitted a project there is another challenge. You task is to create a to do list using tkinter. It should display the tasks you need to complete, as well as a way to either label or remove the tasks you have already completed. You are welcome to complete this challenge in a group or individually. 

