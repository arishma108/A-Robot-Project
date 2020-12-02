# Robot
Build a mail-delivery robot picking up and dropping off parcels.

# Meadowfield
The village of Meadowfield isn’t very big. It consists of 11 places with 14 roads between them. The network of roads in the village forms a graph. The graph will be a collection of points (places in the village) with lines between them (roads). This graph will be the world that our robot moves through. We’re interested in the destinations that we can reach from a given place. 

# The task
Our robot will be moving around the village. There are parcels in various places, each addressed to some other place. The robot picks up parcels when it comes to them and delivers them when it arrives at their destinations.

The automaton must decide, at each point, where to go next. It has finished its task when all parcels have been delivered. To simulate this process, we must define a virtual world that can describe it. This model tells us where the robot is and where the parcels are. When the robot has decided to move somewhere, we need to update the model to reflect the new situation. Condense the village’s state down to the minimal set of values that define it. There’s the robot’s current location and the collection of undelivered parcels, each of which has a current location and a destination address. That’s it.
