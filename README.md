# Cellworld Arena Assembly
All parts of the arena can be found in STEP files of this github repository. However, to see how the parts assemble on 
a web browswer, you can use this [Onshape link](https://cad.onshape.com/documents/c8897f9f1e8291dd2da7ef89/w/1c35d23167742132946594eb/e/1fb43747d3ac53d540c92c7f?renderMode=0&uiState=64f8d54faca3cb0d59202402z).

Files in this repository are based on the Onshape CAD file system where we designed components in part studios and then imported them into assemblies 
to determine their interaction with other parts. Assemblies will be good on visualizing how components are placed together for construction. 
When using the Onshape link, the assemblies will be the first files you see within the files, and
you can both manipulate objects within the assemblies and export them (as well are parts from the part studios) to whatever file you need. 
For creating drawings for laser cutting or STL files for 3D printing however, we recommend using our part studios files.

Components of the arena can be devised into three components: the arena itself, the automated door system, the obstacles, and the water feeder system. 
Construction within each of these categories will be described below, but all parts are derived from either laser-cut acrylic or 3D printing.
Parts that need to be 3D printed will have the string "3D_PRINT" inserted at the beginning of the part's name. 
Step files will have multiple parts included in them.

## The Arena
General construction of the arena will consist primarily of laser-cut parts with exception to the wall binders which we
use to hold the walls together. 11.11 mm diameter neodymium magnets (D74-N52, K&J Magnetics, Pipersville, PA, USA) are 
placed into the floor to hold obstacles in place. Please use the "Final Arena.step"  to grab all the parts. The one arena wall
opposite of the return chute is replaced by the "Human Door.step"  to allow for easy entry of the researcher. 
Please refer to the "Cellworld Arena.step" file in the "Assemblies" folder to see how all parts should fit.

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
"START Door Frame.step", "START flag support.step", "START inner door support"