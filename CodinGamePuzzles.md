### Onboarding Puzzle
```.py
# game loop
while 1:
    enemy_1 = input()  # name of enemy 1
    dist_1 = int(input())  # distance to enemy 1
    enemy_2 = input()  # name of enemy 2
    dist_2 = int(input())  # distance to enemy 2

    # Write an action using print

    # Enter the code here
    
    if dist_1 < dist_2:
        print(enemy_1)
    else:
        print(enemy_2)
```

### The Descent
```.py
mport sys
import math

# The while loop represents the game.
# Each iteration represents a turn of the game
# where you are given inputs (the heights of the mountains)
# and where you have to print an output (the index of the mountain to fire on)
# The inputs you are given are automatically updated according to your last actions.


# game loop
while True:
    max_i=0
    max_h = 0
    for i in range(8):
        mountain_h = int(input())  # represents the height of one mountain.
        if mountain_h > max_h:
            max_h = mountain_h
            max_i = i

    # The index of the mountain to fire on.
    print(max_i)
```

### The Power of Thor Episode 1
```.py
import sys
import math

# light_x: the X position of the light of power
# light_y: the Y position of the light of power
# initial_tx: Thor's starting X position
# initial_ty: Thor's starting Y position
light_x, light_y, initial_tx, initial_ty = [int(i) for i in input().split()]

# game loop
while True:
    remaining_turns = int(input()) 
    move = ""
    if initial_ty > light_y and initial_ty > 0:
        initial_ty -= 1
        move += "N"
    elif initial_ty != light_y and initial_ty < 17:
        initial_ty += 1
        move += "S"
    if initial_tx > light_x and initial_tx > 0:
        initial_tx -= 1
        move += "W"
    elif initial_tx != light_x and initial_tx < 39:
        initial_tx += 1
        move += "E"# The remaining amount of turns Thor can move. Do not remove this line.

    # Write an action using print
    # A single line providing the move to be made: N NE E SE S SW W or NW
    print(move)
```
