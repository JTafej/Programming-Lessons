### Today we will learn about LISTS in python! How exciting... 
#### Here is a website that has a lot of helpful information about lists in python: https://www.w3schools.com/python/python_lists.asp

#### If you had a lot of data to deal with, the lists you use might be extremely long. We will start with some simple lists. 


```
# This is an example of list with 3 elements. 
ages =  [19, 26, 23]

print(ages)
print(ages[1])

# Output:
[19, 26, 23]
26
```
### Notice that when we select the element [1] in "ages" we get the second element. That is because lists start at 0. Below I am providing you with a number of things you can do with lists. Add print(my_list) to see the changes that are made with each piece of code. 
#### Retrieve Elements from the list
```
my_list = [10, 20, 30, 40, 50]
element = my_list[2]  # Accesses the third element (30)
```
#### Change the value of an element in the list
```
my_list = [10, 20, 30, 40, 50]
my_list[1] = 25  # Modifies the second element to 25
```
#### Add elements to the end of a list. 
```
my_list = [10, 20, 30, 40, 50]
my_list.append(60)         # Appends 60 to the end
my_list.extend([70, 80])   # Extends the list with [70, 80]
```
#### Remove elements from a list by value or index(location in the list).
```
my_list = [10, 20, 30, 40, 50]
my_list.remove(40)   # Removes the element with the value 40
del my_list[2]       # Removes the third element (30)
```
#### Sorting
```
my_list = [10, 20, 30, 40, 50]
my_list.sort()  # Sorts the list in ascending order
```
#### If your list is super long, you might not be able to simply count how long the list is. This code will determine the length of the list. 
```
my_list = [10, 20, 30, 40, 50]
length = len(my_list)  # Gets the length of the list
```
#### To check for the existence of an element: 
```
my_list = [10, 20, 30, 40, 50]
if 30 in my_list:
    print("30 is in the list")
```

### Below is an example of code that will write a to-do list in python. We have learned about most (not all) of the code involved in this project. Take a minute to play with it and try to figure out what the different parts are doing. 

```
# Initialize an empty to-do list
to_do_list = []

# Function to add a task to the to-do list
def add_task(task):
    to_do_list.append(task)
    print(f"Task '{task}' has been added to the to-do list.")

# Function to mark a task as completed
def mark_completed(task):
    if task in to_do_list:
        to_do_list.remove(task)
        print(f"Task '{task}' has been marked as completed.")
    else:
        print(f"Task '{task}' not found in the to-do list.")

# Function to display the current to-do list
def display_to_do_list():
    print("To-Do List:")
    for index, task in enumerate(to_do_list, start=1):
        print(f"{index}. {task}")

# Main program loop
while True:
    print("\nOptions:")
    print("1. Add a task")
    print("2. Mark a task as completed")
    print("3. Display the to-do list")
    print("4. Quit")

    choice = input("Enter your choice (1/2/3/4): ")

    if choice == "1":
        task = input("Enter the task you want to add: ")
        add_task(task)
    elif choice == "2":
        task = input("Enter the task you want to mark as completed: ")
        mark_completed(task)
    elif choice == "3":
        display_to_do_list()
    elif choice == "4":
        print("Goodbye!")
        break
    else:
        print("Invalid choice. Please select 1, 2, 3, or 4.")
```




