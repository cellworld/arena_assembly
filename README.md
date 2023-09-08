# Cellworld Arena Assembly
<!-- ![Alt Text](https://github.com/cellworld/arena_assembly/blob/main/Images/cellworld_components-01.png) -->
<p align="center">
  <img src="https://github.com/cellworld/arena_assembly/blob/main/Images/cellworld_components-01.png" alt="arena_overview" width="600" height="381">
</p>

All parts of the arena can be found in the STEP files of this github repository. <b>However, to see how the parts assemble on 
a web browswer, you can use this [Onshape link](https://cad.onshape.com/documents/c8897f9f1e8291dd2da7ef89/w/1c35d23167742132946594eb/e/1fb43747d3ac53d540c92c7f?renderMode=0&uiState=64f8d54faca3cb0d59202402z)</b>.

Files in this repository are based on the Onshape CAD file system where we designed components in part studios and then imported them into assemblies 
to determine their interaction with other parts. Assemblies are good for visualizing how components are placed together for construction. 
When using the Onshape link, the assemblies will be the first files you will see, and
you can both manipulate objects within the assemblies and export them (as well are parts from the part studios) to whatever file format you need. 
For creating drawings for laser cutting or STL files for 3D printing however, we recommend using our part studios files.

Components of the arena can be devised into four components: the arena itself, the automated door system, the obstacles, and the water feeder system. 
Construction within each of these categories will be described below, but all parts are derived from either laser-cut acrylic or 3D printing.
Parts that need to be 3D printed will have the string "3D_PRINT" inserted at the beginning of the part's name.
Step files will have multiple parts included in them.

## The Arena
The arena consists of the arena floor, arena walls, general chamber structures, and the return chute. 
Please use the *Final Arena.step*  to grab all the parts. The one arena wall
opposite of the return chute center is replaced by the *Human Door.step* to allow for easy entry of the researcher. 

With exception to the wall binders (which are 3D printed), all parts are cut from white acrylic. All chamber and return chute components (the walls and ceilings) 
use 3.175 mm thick white acrylic, but all other parts use 6.35 mm thick white acrylic.

Please refer to the *Cellworld Arena.step* file in the *Assemblies* directory to see how all parts should fit.

Specialized Parts:
* 11.11 mm diameter neodymium magnets (D74-N52, K&J Magnetics, Pipersville, PA, USA)
* Red light bulbs (LED Red light therapy bulb, Wolezek LED, China)
* Full spectrum growth lights (9-Watt LED Grow Light Bulb, General Electric, Boston, MA, USA)
* UV light bulbs (UV LED Black lights Bulb, SHGPODA, Shenzhen, Guangdong, China)
* White noise generator (LectroFan Classic, Campbell, CA, USA)

Construction:
1. Assemble floor panels together and insert magnets into floor slots with superglue.
2. Assemble *Human Door.step* using 80/20 25.4 mm aluminum as a frame. Hinges can be added to the aluminum frame for the door.
2. Slot walls and human door into the floor.
2. Attach 3D-printed wall binders using bolts to connect walls together.
3. Add layer of hand-cut clear vinyl (to the shape of the arena) over arena floor.
4. Seal connections between arena walls and 3.175 mm thick clear vinyl floor with silicone sealant.
5. Slot chamber walls and return chute walls into floor.
6. Seal connections between chamber/return chute walls and the floor with silicone sealant.
7. Attach chamber and return chute ceilings. For return chute ceilings we added sticky magnets to the outside of the
arena walls and to the return chute ceiling for easy attachment.
8. Bond introduction chamber walls (minus the "Introduction Sliding Wall") together with the introduction chamber floor using liquid solvent for acrylic bonding (#4 Acrlyic Adhesive, Weld-On, Compton, CA, USA).
9. Insert magnets using superglue into "Introduction Chamber Wall" and the "Introduction Door Blocker".
10. Place light bulbs in the softbox and place in the arena.
11. Mount white noise generator near arena and above the arena walls.

## The Door System
This is the most complex component of the arena to assemble. Three main STEP files will be used to create the structure of the doors:
*END Door Housing.step*, *START outer door support.step*, and *START inner door support.step*. 
To note, all these components are associated with either the START or END chamber (indicated by their name), 
however, all parts can work with both chambers as they are simply mirrored before construction. 
In many cases, this might mean simply flipping parts during assembly.

Files labeled as the "door support" are the components that hold the 
DC motors, limit switches, and silicone/laser cut doors, keeping them in place so that the gear on the motors precisely interacts with the rail inserted into the doors. 
There are two doors associated with each chamber: inner doors control movement between the arena and chamber while outer doors control movement between
the chambers and the return chute. The door supports are housed in one large "door housing" that prevents the mouse
from interacting with electronic components. 

All parts are either 3D-printed or laser-cut using 3.175 mm thick white acrylic. 
To see how everything is assembled, refer to  *Full Door Setup.step* in the *Assemblies* directory,
but note that this is showing the assembly for the END chamber (mirrored to the part studio files). 

Specialized Parts:
* DC motors (50:1 6V micro metal gearmotor, Pololu, Las Vegas, NV, USA)
* Plastic motor holders (Micro Metal Gearmotor Bracket Extended Pair, Pololu, Las Vegas, NV, USA)
* DC motor gear hubs (Universal Aluminum Mounting Hub for 3mm Shaft, M3 Holes, Pololu, Las Vegas, NV, USA)
* Motor driver (DRV8833 Dual Motor Driver Carrier, Pololu, Las Vegas, Nevada, USA, part no. 2130)
* Limit switches (Micro Limit Switch 3Pins, TIAIHUA, China)

Construction:
1. Mirror *END Door Housing.step* and cut parts.
2. Assemble mirrored *END Door Housing.step*.
   1. Bond together all parts except for the "roof" and "ArenaEnclosure" parts using liquid solvent for acrylic bonding (#4 Acrlyic Adhesive, Weld-On, Compton, CA, USA)
and superglue (for when parts need more support).
   2. Bond together all "ArenaEnclosure" parts.
   3. Slot in roof, but leave this unglued.
3. Assemble *START outer door support.step*.
   1. Bond together all acrylic parts of the outer door support. 
   2. Insert limit switches into "3D_PRINT Switch Holder" such that the button is facing towards open slot, securing with screws. 
   3. Bolt down limit switch holder to bonded door support structure.
   4. Attach the "3D_PRINT DC Motor Spacer" by slotting it into the door support. 
   5. Attach the Pololu DC motor gear hubs to the Pololu DC motors. 
   6. Screw down the *3D_PRINT DC_Gear.step* into the gear hubs and motor using M3 screws. 
   7. Place motor on top of the spacer/door support and add the Pololu plastic motor holders, bolting them with the provided Pololu nuts and bolts. 
   8. Superglue *3D_PRINT DC_Teeth.step* into open slot of "Outer Door Silicone Holder" in *Outer Door.step*. 
   9. Superglue 1.5875 mm thick white neoprene rubber cut to the size of the "Silicone Extension" in *Outer Door.step* to the "Outer Door Silicone Holder". 
   10. Slide the assembled *Outer Door.step* into the door support. 
   11. Insert bolt into *Outer Door.step* and secure with nut. Bolt should be able to press limit switches as the door goes up and down. 
4. Assemble *START inner door support.step*
   1. Bond together all acrylic parts of the outer door support except the "Inner Door Silicone Holder". 
   2. Insert limit switched into "3D_PRINT Switch Holder", securing with screws. 
   3. Bolt down limit switch holder to bonded door support structure. 
   4. Attach the "3D_PRINT DC Motor Spacer" in *START outer door support.step* by slotting it into the door support. 
   5. Attach the Pololu DC motor gear hubs to the Pololu DC motors. 
   6. Screw down the *3D_PRINT DC_Gear.step* into the gear hubs and motor using M3 screws. 
   7. Place motor on top of the spacer/door support and add the Pololu plastic motor holders, bolting them with the provided Pololu nuts and bolts. 
   8. Superglue *3D_PRINT DC_Teeth.step* into open slot of "Inner Door Silicone Holder". 
   9. Superglue 1.5875 mm thick white neoprene rubber to the "Inner Door Silicone Holder"
   10. Slide the assembled "Inner Door Silicone Holder" into the door support. 
   11. Insert bolt into the "Inner Door Silicone Holder" and secure with nut. Bolt should be able to press the limit switch when the door is moving down. 
5. Wire motors and limit switches based on *door_water_feeder_electronics.zip* in the *Electronics* directory, making sure that wires connecting limit switches and motors to the motor drivers
are detachable. 
6. Insert the assembled mirrored *END Door Housing.step* (from step 2i; without the "ArenaEnclosure" and roof) into the START chamber. 
7. Insert the assembled *START outer door support.step* and *START inner door support.step* into the Door Housing.
8. Add the "ArenaEnclosure" of the mirrored *END Door Housing.step* (from step 2ii) around *START inner door support.step* and attach roof. 
9. Connect the limit switches and motors to the motor drivers. 
10. Repeat steps 1-9 for the END chamber using mirrored START parts.

## The Obstacles
All obstacles are laser cut using 6.35 mm thick white acrylic. 
To see how everything is assembled, refer to  *Exploded Obstacle.step* in the *Assemblies* directory.

Specialized Parts:
* 11.11 mm diameter neodymium magnets (D74-N52, K&J Magnetics, Pipersville, PA, USA).

Construction:
* For each obstacle, laser cut 1 "Occlusion Base", 1 "Occlusion Top", and 6 "Occlusion Walls".
* Attach magnets into the "Occusion Base" using super glue
* Assemble and bond all parts together using liquid solvent for acrylic bonding (#4 Acrlyic Adhesive, Weld-On, Compton, CA, USA).

## The Water Feeders
All water feeder parts listed in this repository are 3D-printed. 

Specialized Parts:
* Solenoids 
  * We use this solenoid: 2-way Normally Closed Isolation Valve, part number 161T012, NResearch, West Caldwell, NJ, USA
  * However, we recommend using these (this may require changes to the solenoid holder part): 
  Miniature Solenoid Valves Normally Closed 24V, part number 5001T36, McMaster-Carr, Elmhurst, IL, USA
* Capacitive Sensor (AT42QT1011, SparkFun, Boulder, CO, USA)
* Water Spout (Curved Feeding Needles 18 Gauge, part number FNC-18-2-2, Kent Scientific, Torrington, CT, USA)
* Tubing (Tygon S3 E-3603, 1/16 in Inside Dia. 1/8 in Outside Dia., Saint-Gobain, Courbevoie, France)
* Mosfet (RFP30N06LE 30A 60V N-Channel Power Mosfet, WeiMeet, China)

Construction:
1. Place a 60mL syringe, into the *3D_PRINT Water Reservoir Holder.step*
2. Secure the water reservoir 1m above the ground.
3. Place solenoid inside *3D_PRINT Solenoid Holder.step*
4. Secure the solenoid ~30cm above the ground between water reservoir and chamber 
5. Attach wire to water spout using heat shrink wrap. 
6. Secure *3D_PRINT Feeder Holder.step* to chamber walls and insert water spout. 
7. Attach tubing between water spout, solenoid, and water reservoir. 
8. Connect electronics based on *door_water_feeder_electronics.zip* in the *Electronics* directory.
9. Repeat steps 1-8 for other chamber.

## Electronics
<!-- ![Alt Text](https://github.com/cellworld/arena_assembly/blob/main/Images/maze1_circuit_diagram.png) -->
<p align="center">
  <img src="https://github.com/cellworld/arena_assembly/blob/main/Images/maze1_circuit_diagram.png" alt="circuit_diagram" width="600" height="351">
</p>

For connecting all systems together, please follow the EAGLE circuit diagram shown in *door_water_feeder_electronics.zip*.

Specialized Parts:
* Raspberry Pis (3B+, Raspberry Pi, Cambridge, England, UK)


## Code
Relevant code for the arena doors and water feeders resides in separate repositories:

* Code installed on Raspberry Pis (creates services for doors and the water feeder):
[https://github.com/germanespinosa/cellworld_habitat_pi](https://github.com/germanespinosa/cellworld_habitat_pi)
* Terminal to control and connect to doors and water feeder:
[https://github.com/germanespinosa/cellworld_habitat_controller](https://github.com/germanespinosa/cellworld_habitat_controller)
