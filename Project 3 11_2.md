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
