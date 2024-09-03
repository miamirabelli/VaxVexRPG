# Introduction
After my internship ended, I decided to spend my last month of summer fulfilling a longtime goal of mine and making a video game in Unreal Engine 5.

I'm a big fan of Critical Role, so this game is largely inspred by two characters from CR's first campaign: the twins Vax and Vex.

This is my first attempt at a video game in Unreal Engine 5.

# What is this game?
As Vax and Vex are both rogues, this game is a third person RPG with an emphasis on stealth and assassination. Currently, the player controls a character who spawns near a near-abandoned medieval town
(inspired by the Bramblewood Forest). The player can find three different kinds of weapons with different attributes and abilities. The player "wins" the level by defeating the Fort Commander.

## Locomotion
The locomotion system consists of 5 key components: jogging, sprinting, vaulting, climbing, and crouching.

Jogging is the player's default locomotive state.
### Sprinting
The player moves faster while sprinting (currently bound to the ctrl key on Mac). However, sprinting drains stamina.
### Vaulting
The player can vault over obstacles of up to half their height. This is faster and more accurate than simply jumping over these obstacles. Vaulting is implemented using Motion Warping, 
so they can still be attacked and detected while vaulting. Much like sprinting, vaulting costs stamina.
### Climbing
Much like vaulting, climbing is implemented using motion warping. The player can climb up any static mesh that is taller than them---including nonuniform meshes. The player's motion and animation
will smoothly adjust accordingly depending on the angle at which they are climbing.

Once the player reaches the top of wherever they are climbing, they will mantle on to the mesh and continue walking. Mantling costs stamina.
### Crouching
Crouching is the bread-and-butter of the stealth aspect of the game. You are quieter and less visible by AI when you are crouching. However, you cannot attack or sprint.

## Equipment & Weapons
This game has three core kinds of weapons: the dagger, sword, and bow. Attacking with these weapons drains stamina. You can also distract enemies with a rock.
### The Dagger
Daggers are essential for stealth. They do a small amount of damage when in active combat, but they can instantly take out an enemy if you sneak up on them. In addition, assassinating an enemy
doesn't alert other enemies. Daggers are Vax's signature weapon in Critical Role.
### The Sword
Swords are much better than daggers in melee combat; however, you cannot assassinate with them. They do much more damage in close combat, and you can perform devastating combos.
### The Bow
Bows are currently the only projectile weapon in the game, allowing the player to strike from a distance. Arrows do more damage depending on where they strike the enemy. In addition, bows
can be quite stealthy if you play correctly. Bows are Vex's signature weapon in Critical Role.
### The Rock
Rocks don't do any damage, but they are incredibly useful. They can distract an AI via hearing, causing it to investigate a certain area. You can sneak past this distracted AI or creep up to it for a sneak attack.

## AI
This game has two main kinds of AI: regular enemies and bosses.
### Regular Enemies
Regular enemies wield either swords or daggers. These enemies can be assassinated if you sneak up behind them. They can also be distracted by throwing a rock.
### Bosses
Bosses are very formidable, with increased health and attack power. However, they are slower than regular AI. Bosses cannot be distracted or snuck up on, nor can they be assassinated.

# What's next?
Soon, I want to implement a dual-protagonist system where you can switch between Vax and Vex at any point, using their signature skills to complete puzzles and complete missions. While the player
is controlling Vax or Vex, the other twin will be AI-controlled.

To make the game more faithful to Critical Role, I want to add Trinket the Bear, Vex's animal companion. Vex will be able to command Trinket in battle.
# Assets Used & Acknowledgements
## Thanks
Many thanks to Gorka Games and his community discord for helping through my first adventure into game development. Their support helped me learn Unreal Engine 5 quickly.
## Assets
All assets used were free for commercial use with credit. If not mentioned here, the asset was found in the Unreal Engine Store.

[Bow and Arrow Icon](https://www.flaticon.com/free-icon/bow-and-arrow_1423715?related_id=1423715&origin=pack)

[Sword Icon](https://www.flaticon.com/free-icon/sword_1423706?related_id=1423706&origin=pack)

[Dagger Icon](https://www.flaticon.com/free-icon/knife_1423702?related_id=1423702&origin=pack)

[Dagger Asset](https://sketchfab.com/3d-models/cool-dagger-cedc0265c30949a0971700d94af90aed#download)

[Sword Asset](https://sketchfab.com/3d-models/sword-07463a2658e04d6ab8a42b5639a35d63)

[Bow Asset](https://sketchfab.com/3d-models/wooden-bow-free-a762abcffc27478caf19dfaac086485d)

[Crosshair Icon](https://www.flaticon.com/free-icon/crosshair_487009?term=crosshair&page=1&position=32&origin=tag&related_id=487009)
