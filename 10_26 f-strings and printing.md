### f-strings practice. 

#### Here are a couple of the examples from the powerpoint. Please try them out on your own. Mess around with them a bit to see how they work.
##### This is adding two numbers. 
```
x = 5
y = 7
print(f"The sum of {x} and {y} is {x + y}.")
```


##### This is rounding the value of pi to 2 decimals. 
```
pi = 3.14159265359
print(f"The value of π (pi) is approximately {pi:.2f}.")
```
##### This is only printing the first 5 characters of the strings "Hello, World!"
```
text = "Hello, World!"
print(f"First 5 characters: '{text[:5]}'")
```
##### This is letting the user know if it sunny or cloudy and if the weather is warm or cold. Notice how different the syntax is from examples we have seen!
```
temperature = 22
weather = "sunny" if temperature > 20 else "cloudy"
print(f"Today's weather is {weather}. It's {'warm' if temperature > 20 else 'cool'}.")
```
##### This will print todays date using the datetime library. 
```
from datetime import datetime
today = datetime.now()
print(f"Today's date: {today:%Y-%m-%d}")
```
#### Please note: , the percent signs within the f-string are used to indicate formatting directives. They are not part of the f-string syntax but rather part of the formatting syntax specific to the datetime module. In this case, the percent signs are used to specify how the today variable, which is a datetime object, should be formatted as a string.

### Your task for today is to create a madlibs game like the one we played during the introduction today. You will need to ask the user for adjectives, verbs, nouns, and adverbs that will fit into your story. 








