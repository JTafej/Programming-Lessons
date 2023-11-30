## In a group of two, use this code and find the RGB values that correspond to the color on the board. 

```
import pygame

pygame.init()

SCREEN_WIDTH = 800
SCREEN_HEIGHT = 600

screen = pygame.display.set_mode((SCREEN_WIDTH, SCREEN_HEIGHT))
wall1 = pygame.Rect((140, 80, 500, 20))
player = pygame.Rect((30, 250, 20, 20))
run = True
while run:

  screen.fill((R,G,B))

  for event in pygame.event.get():
    print(event)
    if event.type == pygame.QUIT:
      run = False

  pygame.display.update()

pygame.quit()
```



