# aaa123
from pygame import *
mixer.init()
window = display.set_mode((700, 500))
display.set_caption("Лабиринт")
background = transform.scale(image.load("background.jpg"), (700, 500))

class GameSprite:
    hero = transform.scale(image.load("hero.png"), (100, 100))
    cyborg = transform.scale(image.load("cyborg.png"), (100, 100))
    treasure = transform.scale(image.load("treasure.png"), (50, 50))
clock = time.Clock()
FPS = 60
game = True
while game:
    for e in event.get():
        if e.type == QUIT:
            game = False
    if game != False:
        if  sprite.collide_rect(hero, final)
            font.Font(None, 70)
            win = font.render("YOU WIN!", True, (255, 215, 0))
            window.blit(win, (200, 200))
            money = mixer.Sound('money.ogg')
            finish = True
        money.play()
        if sprite.collide_rect(hero, cyborg) or sprite.collide_rect(hero, wall)
            font.Font(None, 70)
            lose = font.render("YOU LOSE!", False, (255, 215, 0))
            window.blit(lose, (200, 200))
            kick = mixer.Sound('kick.ogg')
        kick.play()


        window.blit(background,(0,0))
        window.blit(hero, (500, 150))
        window.blit(cyborg, (400, 200))
        window.blit(treasure, (550, 350))

        display.update()
        clock.tick(FPS)
mixer.music.load('jungles.ogg')
class Player(GameSprite):
def __init__(self)
    keys_pressed = key.get_pressed()
        self keys_pressed[K_UP]
            y = -10
        self keys_pressed[K_DOWN]
            y = +10
        self keys_pressed[K_LEFT]
            x = +10
        self keys_pressed[K_RIGHT]
            x = -10
    update()

class Enemy(GameSprite):
def __init__(self)
    keys_pressed = key.get_pressed()
        self keys_pressed[K_LEFT]
            x = +10
        self keys_pressed[K_RIGHT]
            x = -10
    update()

class Wall1(Sprite):
    def __init__(self, rect, fill, blit):
        self window.blit(wall1, (50, 160))
        self image = Surface((2, 2))
        self image.fill(100, 100, 100)
        self rect = image.get_rect()
    update()
    

class Wall2(Sprite):
    def __init__(self, rect, fill, blit):
        self window.blit(wall2, (160, 50))
        self image = Surface((2, 2))
        self image.fill(100, 100, 100)
        self rect = image.get_rect()
    update()
    

class Wall3(Sprite):
    def __init__(self, rect, fill, blit):
        self window.blit(wall3, (80, 80))
        self image = Surface((2, 2))
        self image.fill(100, 100, 100)
        self rect = image.get_rect()
    update()
