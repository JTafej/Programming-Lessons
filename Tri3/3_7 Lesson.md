### Warm-up. For your warm-up today, you will get into groups of two again. Each person will take turns writing. 
#### First challenge: Write a Python function that converts temperature from Celsius to Fahrenheit and vice versa. The conversion formulas are:
* F = (9/5)*C + 32
* C = (5/9)(F - 32)

#### Second Challenge: Write a Python function that converts distance measurements between different units. The function should support conversion between kilometers, miles, meters, and feet. The conversion formulas are: 
* 1km = 0.621 Miles
* 1 meter = 3.281 feet



### Today we are going to highlight the distinction between dictionaries and lists!
#### Remember, dictionaries are key-value pairs, and lists are ordered collections of elements.
```
# Example of a dictionary and a list
student_scoresdictionary = {'Alice': 85, 'Bob': 92, 'Charlie': 78}
fruitslist = ['apple', 'banana', 'orange', 'pear']
```
#### We can also COMBINE dictionaries as lists, as in the following example: 

```
# Example: Store information about students in a list of dictionaries
students = [
    {'name': 'Alice', 'score': 85},
    {'name': 'Bob', 'score': 92},
    {'name': 'Charlie', 'score': 78}
]
```

#### If we want to access or adjust items that are in a dictionary, within a list, we can use the following: 
```
# Example: Accessing and manipulating data in a list of dictionaries
print(students[0]['name'])      # Output: 'Alice'
students[1]['score'] = 95       # Update Bob's score
students.append({'name': 'David', 'score': 88})  # Add a new student
```

### Now for the challenge: 
####  Student Management System (30 minutes):

#### Get into groups of 2 or 3, and create a simple student management system using dictionaries and lists. The system should allow adding new students, updating scores, and displaying student information.

#### When all groups have a finished product, you will have a change to share at the end of the day. 



