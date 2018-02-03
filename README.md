# flying-dots


Dennis Zethof - Februari 2018

v0.4

NOTE: This version is setup to show that the collision
detection works, and can be started and left alone indefinite.
The code aims to handle collisiondetection independent of
the amount of calculationcycles per second (main_loop_interval). 
It checks for collisions, handles the one that occurs first up
to the point of collision, calculates the effects, evaluates the 
new situation, and then handles the resulting earliest next 
collision.

By all means this code is not finished. It is too inefficient to
do what it is supposed to: run until the box is fully filled 
with dots. In order to achieve this a more efficient way of 
collision detection must be employed; this version uses a mostly
iterative process, so when set at .001, each potential collision
will trigger a 1000 checks. A grid system is in place to limit
the number of times the checking system is triggered, which is a
sort of sweeping type of algorithm, but it it is not enough. It 
should be done much more efficient AND much more precise by using 
a collision detection method that relies more on mathematics.

TODO: 

   	- heavy refactoring
    
   	- change collision detection system
    
   	- add polynomial options
 
NICE TO HAVES:

	  - rotation of objects
