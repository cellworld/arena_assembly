# Cellworld Arena Assembly
All parts of the arena can be found in STEP files of this github repository. However, to see how the parts assemble on 
a web browswer, you can use this [Onshape link](https://cad.onshape.com/documents/c8897f9f1e8291dd2da7ef89/w/1c35d23167742132946594eb/e/1fb43747d3ac53d540c92c7f?renderMode=0&uiState=64f8d54faca3cb0d59202402z).

Files in this repository are based on the Onshape CAD file system where we designed components in part studios and then imported them into assemblies 
to determine their interaction with other parts. Assemblies are good for visualizing how components are placed together for construction. 
When using the Onshape link, the assemblies will be the first files you see within the files, and
you can both manipulate objects within the assemblies and export them (as well are parts from the part studios) to whatever file format you need. 
For creating drawings for laser cutting or STL files for 3D printing however, we recommend using our part studios files.

Components of the arena can be devised into three components: the arena itself, the automated door system, the obstacles, and the water feeder system. 
Construction within each of these categories will be described below, but all parts are derived from either laser-cut acrylic or 3D printing.
Parts that need to be 3D printed will have the string "3D_PRINT" inserted at the beginning of the part's name.
Step files will have multiple parts included in them.

## The Arena
The arena consists of the arena floor, arena walls, general chamber structures, and the return chute. 11.11 mm diameter neodymium magnets (D74-N52, K&J Magnetics, Pipersville, PA, USA) are 
placed into the floor to hold obstacles in place. Please use the *Final Arena.step*  to grab all the parts. The one arena wall
opposite of the return chute is replaced by the *Human Door.step*  to allow for easy entry of the researcher. 
With exception to the wall binders (which are 3D printed), all parts are cut from white acrylic. All chamber and return chute components (the walls and ceilings) 
use 3.175 mm thick arcylic, but all other parts use 6.35 mm thick acrylic.


Please refer to the *Cellworld Arena.step* file in the *Assemblies* folder to see how all parts should fit.

Construction:
1. Assemble floor panels together and insert magnets into floor slots with superglue
2. Assemble Human Door.step using 80/20 1-in aluminum as a frame
2. Slot walls and door into the floor
2. Attach 3D-printed wall binders using bolts to connect walls together
3. Add layer of hand-cut clear vinyl over arena floor
4. Seal connections between arena walls and the floor with silicone sealant
5. Slot chamber walls and return chute walls into floor
6. Seal connections between chamber/return chute walls and the floor with silicone sealant
7. Attach chamber and return chute ceilings. For return chute ceilings we added sticky magnets to the outside of the
arena walls and to the return chute ceiling for easy attachment.
8. Bond introduction chamber walls (minus the "Introduction Sliding Wall") together with the introduction chamber floor using liquid solvent for acrylic bonding (#4 Acrlyic Adhesive, Weld-On, Compton, CA, USA).
9. Insert magnets using superglue into "Introduction Chamber Wall" and the "Introduction Door Blocker"

## The Door System
This is the most complex component of the arena to assemble. Three main STEP files will be used to create the structure of the doors:
*START Door Frame.step*, *START outer door support.step*, *START inner door support.step*. 
To note, all these components are associated with the START chamber, however, all parts can work with the END door as well as
they are simply mirrored before construction. 

Files labeled as the "door support" are the components that hold the 
DC motors, limit switches, and silicone/laser cut doors, keeping them in place so that the gear on the motors precisely interacts with the rail inserted into the doors. 
There are two doors associated with each chamber: inner doors control movement between the arena and chamber while outer doors control movement between
the chambers and the return chute. The door supports are housed in one large "door frame" that prevents the mouse
from interacting with electronic components. 

All parts are either 3D-printed or laser-cut using 3.175 mm thick white acrylic. 
To see how everything is assembled, refer to  *Full Door Setup.step* in the *Assemblies* folder
but note that this is showing the assembly for the END chamber (mirrored to the part studio files). 

Purchased Parts:
* DC motors (50:1 6V micro metal gearmotor, Pololu, Las Vegas, NV, USA)
* Plastic DC motor holders ()
* DC motor gear thingy ()
* Raspberry Pis (3B+, Raspberry Pi, Cambridge, England, UK)
* H-bridges ()
* Limit switches ()

Construction:
* fefe 
  * fefefef


## Code
Relevant code for the arena doors and water feeders resides in separate repositories:

* Code installed on Raspberry Pis (creates services for doors and the water feeder):
[]
* Terminal to control and connect to doors and water feeder:
[]
