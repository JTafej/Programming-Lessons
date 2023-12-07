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
