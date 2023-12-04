## Today we will continue building the games we started last week. 

```
import pygame

pygame.init()

SCREEN_WIDTH = 800
SCREEN_HEIGHT = 600

screen = pygame.display.set_mode((SCREEN_WIDTH, SCREEN_HEIGHT))
wall1 = pygame.Rect((140, 80, 500, 20))
player = pygame.Rect((300, 250, 20, 20))

def draw_text(text, font, text_col, x, y):
  img = font.render(text, True, text_col)
  screen.blit(img, (x, y))

text_font = pygame.font.SysFont("Helvetica", 30)

run = True

Grey = (200, 200, 200)
Blue = (200, 100, 100)
Col = Grey
Col2 = Blue
while run:
  
  screen.fill((0,0,200))
  if player.colliderect(wall1):
    Col = Col2
    draw_text("YOU LOSE", text_font, (255, 255, 255), 220, 150)
  
  
  pygame.draw.rect(screen, (2,255, 200), player)
  pygame.draw.rect(screen, Col, wall1)
  
  key =pygame.key.get_pressed()
  if key[pygame.K_a] == True:
    player.move_ip(-1, 0)
  if key[pygame.K_d] == True:
    player.move_ip(1, 0)
  if key[pygame.K_w] == True:
   player.move_ip(0, -1)
  if key[pygame.K_s] == True:
        player.move_ip(0, 1)


  
  for event in pygame.event.get():
    print(event)
    if event.type == pygame.QUIT:
      run = False

  pygame.display.update()

pygame.quit()
```
