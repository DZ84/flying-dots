# flying-dots


Dennis Zethof - Februari 2018

	v0.45

	NOTE: The main focus of this specific project is to get the 
	collision detection algorithm right, this is a test setup,
	and by all means not finished. It is not efficient enough,
	and not without bugs. However, right now you can run it
	for quite a while, and I've seen no dots leaving their box
	or overlap eachother (except on their spawning area in the 
	upper left corner, they overlap there at first). The goal is to 
	let the box be fully filled with dots until none can be added. 
	I have removed most of the comments because they would
	clutter the code and where not written to be read by others.	
	
	Algorithms: this code scans all the dots, determines if there 
	will be any collisions, performs the collision earliest in time, 
	reevaluates the new situation caused by the collision, then
	performs the next earliest collision, reevaluates etc.
	
	By default the amount of dots is set at 80, you can easily set
	"settings_maximum_dots" to about 150. Ofcourse that may not run 
	as smooth.

