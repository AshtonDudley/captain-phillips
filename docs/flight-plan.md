# Flight Plan
Run One (Safe dead reckoning, coastal route, electromagnets to handle cargo)

## Navigation
Robot starts with 90 degree scan in starting port
Ultrasonic sensor on the bottom of the robot facing forward. - HAS TO BE LOWER THAN ATTACHED CARGO
Difference between ultrasonic and LIDAR readings can indicate objects (due to LIDAR being too high to pick up object).

### Delivery Route
Avoid all detected objects on the way to the opposite port to drop off initial cargo.
Scan at the starting port, detect any objects
Move forward to next corner.
360 degree scan in next corner for objects.
Move forward to next corner.
Continue this pattern 3 more times until in the opposite port.
Disengage electromagnets

### Retrieval Route
Turn around to go backwards after dropping initial cargo
Engage electromagnets again
Do a 360 scan again from the opposite port
Go towards the direction of the new cargo
Use the increased current draw when magnets attach as a way to detect pick up of cargo
Once cargo is picked up, use lidar to reorient from the opposite port area and start moving backwards
use ultrasonic to avoid the boat, and repeat scanning + dead reckoning back to original port.

### Need to figure out retrieval of life boat (Luc)
