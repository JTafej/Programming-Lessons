## Hi everyone! Welcome back. 

### Today we will continue with our game creation. As the year progresses we will cover other topics, but we will stick with games for a bit. 

### You may need a refresher on how the code works for these basic games. Take a look at the two pieces of code below. See if you are able to combine them to create a snowy scene to move your rectangle through. 

## Using Sprite to create rectangles: 
```
import random
import pygame

# Global Variables
COLOR = (255, 100, 98)
SURFACE_COLOR = (255, 255, 255)
WIDTH = 500
HEIGHT = 500

# Object class
class Sprite(pygame.sprite.Sprite):
  def __init__(self, color, height, width):
    super().__init__()

    self.image = pygame.Surface([width, height])
    self.image.fill(SURFACE_COLOR)
    self.image.set_colorkey(COLOR)

    pygame.draw.rect(self.image,
            color,
            pygame.Rect(0, 0, width, height))

    self.rect = self.image.get_rect()

  def moveRight(self, pixels):
    self.rect.x += pixels

  def moveLeft(self, pixels):
    self.rect.x -= pixels

  def moveForward(self, speed):
    self.rect.y += speed * speed/10

  def moveBack(self, speed):
    self.rect.y -= speed * speed/10


pygame.init()


RED = (255, 0, 0)


size = (WIDTH, HEIGHT)
screen = pygame.display.set_mode(size)
pygame.display.set_caption("Creating Sprite")


all_sprites_list = pygame.sprite.Group()

playerCar = Sprite(RED, 20, 30)
playerCar.rect.x = 200
playerCar.rect.y = 300


all_sprites_list.add(playerCar)

exit = True
clock = pygame.time.Clock()

while exit:
  for event in pygame.event.get():
    if event.type == pygame.QUIT:
      exit = False
    elif event.type == pygame.KEYDOWN:
      if event.key == pygame.K_x:
        exit = False

  keys = pygame.key.get_pressed()
  if keys[pygame.K_LEFT]:
    playerCar.moveLeft(10)
  if keys[pygame.K_RIGHT]:
    playerCar.moveRight(10)
  if keys[pygame.K_DOWN]:
    playerCar.moveForward(10)
  if keys[pygame.K_UP]:
    playerCar.moveBack(10)

  all_sprites_list.update()
  screen.fill(SURFACE_COLOR)
  all_sprites_list.draw(screen)
  pygame.display.flip()
  clock.tick(60)

pygame.quit()

```
## Using lists and loops to create snowfall: 
```
import pygame
import random
pygame.init()

WHITE = [255, 255, 255]
GREEN = [0,255,0]
SIZE = [400, 400]

screen = pygame.display.set_mode(SIZE)
pygame.display.set_caption("Programming World of GFG")

snowFall = []
for i in range(50):
  x = random.randrange(0, 400)
  y = random.randrange(0, 400)
  snowFall.append([x, y])

clock = pygame.time.Clock()
done = False
while not done:

  for event in pygame.event.get(): 
    if event.type == pygame.QUIT: 
      done = True
  screen.fill(WHITE)
  for i in range(len(snowFall)):
    pygame.draw.circle(screen, GREEN, snowFall[i], 2)

    snowFall[i][1] += 1
    if snowFall[i][1] > 400:
      y = random.randrange(-50, -10)
      snowFall[i][1] = y

      x = random.randrange(0, 400)
      snowFall[i][0] = x

  pygame.display.flip()
  clock.tick(20)
pygame.quit()
```
