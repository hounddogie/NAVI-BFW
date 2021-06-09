# NAVI-BFW
This is the code repo for NAVI's BFW framework. 

NAVI is a mech AI project.

Overview.

NAVI is used to integrate navigation in all ranges of appliances.
The main focus of NAVI is strategic combat.

Once implemented, the chip will assess the appliance it is in by characteristics defined (Such as a role)
as well as parameters assessed (physical aspects) and use them for decision making.

The chip will select a master or a team lead of the squad. to command the team of other mechs to carry out actions.
Everything will be fully autonomous.


The mechs will use 4 "beacons" to communicate via relay satelites mounted on the mechs like turrets.
These allow more strategic weakpoints.

The beacons will be relay towers using wire satelite dishes.
The beacons will use means of two way radio to sync location so that the mechs may point their data transferrers to the dishes to sync info
No doubt this will take another e2 script to manage data transfer.

The point of this is to have a good combat environment for players to try crazy acf builds on.
If they cant beat them mechs they can alternatively use strategic disruption of the mechs to possibly single them off since they wont be able to communicate they
will have to work on their own which can lead to vulnerabilities.


more on roles:

------beaconboy-----
initially the beacons will not be in place. a robot will drop these beacons on 4 points of the map
this will also add some interesting aspects to combat. If you are able to kill the beaconboy before he deploys his beacons it will be a great start in battle
since you have prevented the beacons from being deployed, you have separated the mechs from their pack opening vulnerabilities.

------Master--------
This is self explanatory, master is the role of the mech giving commands.
NAVI could depict the strongest mech as master on its own or there could be an override. 

------Scout------
Tis but a pawn. 
Master will assign this one to brush off small opponents or to do basic grunt work.

More to come... still brainstorming.



---------------------------------------
Agenda.
--------------------------------------
Finish up navigation aspect of chip.

Make a serialized function for means of sending commands.
Maybe in the form of a function() that sends the data value
The goal for this task is to make a command that encodes an entire command
in a single data value and can be decoded. must be able to be sent thru wire number output.

Make beacon relay infrastructure that is capable of routing these requests using a network of 
(setang'd and setpos'd) gimbal aimed wire data transferrers

Build a beacon. 
