### Happy Wednesday! Your last project of the year is to create a automatic-mad-libs game. This will involve creating a list of verbs, nouns, and adjectives. After you have your list, you will need to write a string that prints a story with a Random verb, noun, and adjective selected. See the code below to get an idea of a starting place. Notice that the code below prints a string with a random verb or noun. 

```
import random

# List of 20 verbs
verbs = ["run", "jump", "swim", "eat", "sleep", "write", "sing", "dance", "read", "talk", "listen", "laugh", "think", "paint", "climb", "cook", "draw", "drive", "fly", "hike"]

# Select a random verb
random_verb = random.choice(verbs)

# Print the random verb
print(f"Random verb: {random_verb}")

# list or random nouns
nouns = ["dog", "cat", "bird", "fish", "lion", "tiger", "bear", "giraffe", "elephant", "girl", "boy", "man", "woman", "child", "woman", "man", "woman", "child"]

# Select a random noun
random_noun = random.choice(nouns)

# Print the random noun
print(f"Random noun: {random_noun}")

print(f"In walks a {random_noun}. Suddenly, the {random_noun} starts {random_verb}ing!")
```

### If you get done early and you want to do a level 2 project: 
#### Change the program so that it asks the users for the correct number of adjectives, nouns, and verbs and puts them into a list. (You can do this with a for loop, see example below) This will make the program more interactive. 

```
adjectives = []
# lets say you need 4 adjectives: 
for i in range (1, 5):
  adj = input("Please provide an adjective: ")
  adjectives.append(adj)
# to print the whole list
print(adjectives)
# If you want the second term in the list:
print(adjectives[1])

print(f"I went on a walk with {adjectives[1]} friend")
```

### Level 3
#### To add a level of complexity, you should create a 3 different stories, about different topics. You can have the user pick which story they want to use based on the topics. 


