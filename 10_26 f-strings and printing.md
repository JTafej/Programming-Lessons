### f-strings practice. 

#### Here are a couple of the examples from the powerpoint. Please try them out on your own:
```
temperature = 22
weather = "sunny" if temperature > 20 else "cloudy"
print(f"Today's weather is {weather}. It's {'warm' if temperature > 20 else 'cool'}.")
```

```
from datetime import datetime
today = datetime.now()
print(f"Today's date: {today:%Y-%m-%d}")
```
#### Please note: , the percent signs within the f-string are used to indicate formatting directives. They are not part of the f-string syntax but rather part of the formatting syntax specific to the datetime module. In this case, the percent signs are used to specify how the today variable, which is a datetime object, should be formatted as a string.

