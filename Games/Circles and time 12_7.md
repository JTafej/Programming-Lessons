# Today we will continue what we started the last few days. 

### Below is the code for drawing a blue circle on a black background. See if you can use this code to create a new game. You can create a game that is similar, but uses circles as well. Please note that colliderect does not work for circles. We will talk about how to handle collisions of objects other than rectangles 


```
import pygame 
# Initialize Pygame
pygame.init()
# Set the size of the pygame window. 
win = pygame.display.set_mode((500, 500))
# Assign Values
x = 250
y = 250
radius = 50
color = (0,0,255) # RGB values for blue color
# Create a loop to keep the window running
while True:
    pygame.draw.circle(win, color, (x, y), radius)
    pygame.display.flip()
pygame.quit()
```

### Here is an example of how you may add a timer to your program. This first part will go before your game loop begins:
start_time = currenttime.time()

### This next part will go after the user has completed their goal. For example, when they reach the final block. 
```
total_time = currenttime.time() - start_time
time_text = f"Your total time was: {int(total_time)} seconds"
    draw_text(time_text, text_font, (2, 255, 50), 100, 300)
    pygame.display.update() 
```

### Create a new game using this information! You can also use everything we have learned this week about rectangles and collisions. You will create this game in groups today. 
