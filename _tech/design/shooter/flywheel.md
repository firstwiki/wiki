---
title: Flywheel
tags: shooter
---

One type of [shooter](shooter) that features one or several wheels spinning at very high speeds and then have a ball compressed against them. There are several different variables that you can change to alter the performance of the shooter. Commonly these are setup in one of two methods: One or Two flywheel setups.

## Designs

### Single Flywheel

Usually this centers around a single flywheel in the center, or several wheels lined up next to each other in a line. On the outisde of this wheel is a gap large enough for the game piece and then a retaining wall. The exiting angle is determined by where that retaining wall ends on the arc. This style of shooter is usually used on [turrets](turrets).

### Double Flywheel

This setup contains two flywheels that are on each side of a gap that is designed for a size of the game piece being shot. This offers significantly easier adjustment of compression, as with a single flywheel you have to change the radius of the entire setup, but requires you to adjust both wheels's angle if you need to adjust the shooting angle. 

### Other Designs



## Performance

There are several different items that can be added to increase the shooting range of the shooter.

### Compression

By increasing the amount of "squeeze" between the flywheel and the wall. By increasing this compression, the more normal force that is applied to the game piece, and thus the amount of friction that is applied is increased. This results in a higher speed to a certain extent. Too much compression can result in damaged or destroyed game pieces, which will not make field staff happy. This also starts to reduce game piece speed.

### Speed

The amount of speed you have your flywheel at is usually the variable you change the most to adjust the aim of the shooter. By varying the output of the [motor controller](motor-controller), you can adjust the speed. You want to have your speed on a [closed loop](closed-loop-control) so that when your battery voltage reduces during the course of a match, your flywheel speed stays the same. For very much the same reason, you should be testing your flywheel system at about 60% so you can adjust for you lowest battery voltage. Adjusting your compression and maximum motor RPM can increase your area for this. 

Your shooter maximum speed is very dependent on your design, your wheels and your compression. There is no general rule of thumb, it almost entirely depends on your setup. You will need to do shooter testing to make sure it works. 

### Inertia

If you are shooting a large quantity of game objects in a short period, such as in [FIRST STEAMWORKS](first-steamworks), you need to have a high inertia. Inertia determines how much torque is required to accelerate the flywheel. By adding more mass further away from the axle, you can add more rotational inertia. A higher rotational inertia means that the flywheel will take longer to accelerate up to speed, but it also means less speed will be lost every time a game piece is shot. A simple way to increase inertia is to use larger or heavier wheels, but another option is to use a seperate weight either attatched on the same axle or geared seperately like [118 in 2017](https://www.youtube.com/watch?v=x6CtdZ91qzI&feature=youtu.be)

### Wheels

Your wheel choice is most importantly impacted by your game piece. If your game piece is soft and malleable, you can use harder wheels, but if your game piece is harder, you need to use softer wheels so your compression isn't acting against your shooter rotation. Of course you need to think about shooter speed when deciding on wheel size (which can also affect inertia). Durability is also a concern, since these are spinning at such high speeds, you need to have a high durability (which is usually referred to with [durometer](durometer)), but this often results in lower friction. You need to have a good balence between friction and durability, which can be best determined using shooter testing off the robot first.
