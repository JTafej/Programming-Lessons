### Today we will talk about a new type of data structure called dictionaries. We have already discusses lists, which are also a form of data structure in python. 

### Data structures are "containers" that each organize and store data in their own unique way. Lists are a form of data structure that store data in an ordered fashion. In other words, the order of items matters in a list, and can be used to select certain values. Dictonairies, Tuples, and Sets are the other common data structures you may see in python. 

### What is a dictionary? 
#### A dictionary is a general-purpose UNORDERED data structure for storing a group of objects. A dictionary has a set of keys and each key has a single associated value. When presented with a key, the dictionary will return the associated value. 
#### For example, the results of a classroom test could be represented as a dictionary with pupil's names as keys and their scores as the values:

```
results = {'Detra' : 17,
           'Nova' : 84,
           'Charlie' : 22,
           'Henry' : 75,
           'Roxanne' : 92,
           'Elsa' : 29}
```
#### In this case, the names are the keys that we can use to access data. We use those instead of calling on the number in a list. 
```
print(results['Nova'])
84
print(results['Elsa'])
29
```

#### Lets see another example of a useful dictionary. Say we have a phone book:
```
phonebook = {"Alice": "123-456-7890", "Bob": "987-654-3210"}
```

#### We can access Alice's phone number with the following code: 
```
print(phonebook["Alice"])
# Output: 123-456-7890
```

#### We can also add a new number or modify an existing number. (This could also be used for something like passwords...)
```
# Add a new entry
phonebook["Charlie"] = "555-123-4567"
# Update an existing entry
phonebook["Bob"] = "098-765-4321"
```
#### Copy and paste the following example to your replit to test it. You should notice that this dictionary has 3 values associated with each person. You should also notice that nothing is printed when you run this code. The program is simply storing the data at this point. 
```
employees = {
    "John": {
        "department": "Marketing",
        "position": "Manager",
        "salary": 100000
    },
    "Jane": {
        "department": "Sales",
        "position": "Lead",
        "salary": 85000
    }
}
```
#### Now let's say that we want to access John's department. We could use the following code to do this. Try it out! 
```
John_dept=employees["John"]["department"]
print(John_dept)
```

















