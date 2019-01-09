# flying-dots


	Dennis Zethof - Januari 2019

	v0.60

	The main focus of this specific project is to get the
	collision detection algorithm right, this is a test setup,
	and by all means not finished.

	Got it to run quite a bit more efficient. The main 
	improvements were in the functions:

	-get_rounded_number
	-remove_old_grid_positions
	-weave_grids_together
	-check_redo_position (now with hash maps)
	-remove some rounding calls

	Algorithms: this code scans all the dots, determines if there
	will be any collisions, performs the collision earliest in time,
	re-evaluates the new situation caused by the collision, then
	performs the next earliest collision, re-evaluates etc.

	By default the amount of dots is set at 100, you can easily set
	"settings_maximum_dots" to about 150. But that may not run 
	as smooth. Similarly the speed can be adjusted by searching for
	"set_speed".

