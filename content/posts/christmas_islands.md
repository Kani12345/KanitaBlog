+++
authors = ["Kanita"]
title = "Unity game project: Christmas Islands"
date = "2024-10-19"
description = "unity game"
+++


<h1 text-align: center> Unity Game Project: Christmas Islands </h1>  

For my unity class, I had to make a 3D unity game. I chose to do a 3D platformer on the theme of Christmas where the player has to collect all the presents to win. Click [here](/KanitaBlog/posts/Final_Game.zip) if you want to download the game and [there](https://github.com/Kani12345/ChristmasIsland) if you want to see the project on github.
## Finalised game 
The game is divised in three scenes. Upon lanch, the first scene is the menu. 
### Menu 
The menu is very simple. The play button allow the user to play the game and the quit button allow them to quit the application.

<img src="/KanitaBlog/posts/menu_winterisland.png" width= 700>

### Winning Scene 
Upon winning, a simple wining scene is displayed. The user can either play again or quit the application by clicking on the corresponding button. 
<img src="/KanitaBlog/posts/win_image.png" width= 700>

### Game
The goal of the user is to collect the seven christmas presents that are on the platforms. There are some easy game mechanics such as a small platform used as an elevator and some snow to brush off to find a present.
Heres a runthrough of the game:

<video width="700" height="480" controls>
  <source src="\KanitaBlog\posts\finalegame_runthrough.mp4" type="video/mp4">
  <source src="\KanitaBlog\posts\finalgame_runthrough.mp4" type="video/ogg">
Your browser does not support the video tag.
</video>


#### UI
The user interface is pretty simple. 
The player can controll the character through  Q,Z,S,D and space keys and the mouse. The mouse is used to control the direction of vision and displacement. They can use the Q, S, Z, D keys move the player and the space bar to jump. The user can also close the window by clicking on the 'x' button.
At the top left on the window, the number of collected presents is shown clearly so the player knows how many presents he needs to pick up to win the game at all times. 



 
#### The platforms 

##### Platform #1: starting zone
<img src="/KanitaBlog/posts/start_platform.png" width= 700>

##### Platform #2: forest zone 
<img src="/KanitaBlog/posts/forest_platform.png" width= 700>

##### Platform #3: village zone 
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

##### Platform #4: christmas mountain
<img src="/KanitaBlog/posts/christmas_platform.png" width= 700>


## Problems encountered and improvement left  
### Problems encountred 
#### Player jittering after a collision
hWen first implementing the character controller, the character was jittering as seen in the gif
below.
By changing the collider of the platforms from a mesh collider to a box collider, the
character stopped automatically jittering. But it would still jitter when colliding with an object
other than the ground.
By making the camera independant from the player, I could affirm that the jittering
effect was coming from the player and not the camera. The issue seemed to stem from the
physics aspect of the game but it was hard to pinpoint the exact issue.
I started to check on stackoverflow and other websites if people encountered the
same issues and applied the solutions given to them: I checked if the player character's
detection was set to continuous, if in the script moving the character I was updating its
position in the fixed update and not in the update. But most of the solutions were already
implemented in my game and the few that were not didn’t fix this issue.
To try to find the issue, I started doing by project again from scratch and this issue
came back even when the platform was a simple cube and the player was colliding with a
simple object. I was then able to confirm that the issue came from the player. When talking
to my teacher about this issue, she asked me how the player was standing when its collider
was a cylinder. The shape of its collider was the reason behind the jittering. When moving on
a plane surface, the forces applied on the player in the scene were only vertical, therefore
not disturbing its balance. But when a force with vertical component was applied (when
walking on an uneven surface or colliding with an object such as a tree), it would disturb the
balance, therefore causing the jittering. To force the player to stay balanced, I locked the X
and Z rotations, and that solved the whole jittering issue.
<img src="/KanitaBlog/posts/gittering_character.gifùm" width= 700>

### Improvement left 

#### Smoother interaction between the player and the elevator
As seen in the walkthrough of the game, when the character is on the elevator platform, it doesn't stick to it, making the movement jerky. A way to solve that would be making a script that detect when the player is on the platform and make it a child of the platform while it stays on it.

#### Better animations of the character
The animations of the character look a bit weird, espcially when you move the character using the S, Q, D keys. A way to solve that would be to add animations for when the character is walking backwards or sideways. 

#### More accurate mesh colliders and smoother collisions 
The mesh  collideers of the platfoms are a bit approximative, which sometime leads the character to be a few centimeters above the ground. The collisions could also be improved. Both of this issues lead to an awkward feeling when clibing the mountain. 

#### Adding more SFXs
The game could be more immersive if more sfxs where added, such as foosteps sounds when walking, a sound when colliding with an object such as a house or a tree. 





## Ressources used
### Skybox 
### Snow 
### Player 
### Platforms  



