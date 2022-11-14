# vrcloset
## wip resource for modding wearables in Animal Crossing: New Horizons
don't expect too much here for a while, it's literally just messy notes full of typos and formatting errors for now



the step-by-step instrcutions for each clothin type will be very different. i'll be keeping record of the steps i take to achieve certain outcomes here

no models for clothing? these items work just like the custom code clothing does in-game
these clothing types use a separate model because they are 'shared'
models for accessories, shoes, hats etc. will be included in the item file because they are 'unique'


https://gbatemp.net/threads/mario-kart-8-custom-track-tutorial.485627/

'guide'

**switch prerequisits:**
- modded switch (+ all the things)
- nxdumptool-rewrite (+ dependencies)
- dumped romfs from tool above

**pc:**
- toolbox
- blender
- NHSE (or this abandoned project? https://github.com/FluffyFishGames/ACNHDesignPatternEditor/issues/42 With NHSE, you are only able to dump or import as .nhd/.nhpd (abandoned project supports NHSE file types) note on NHSE: These files are formatted the same way as .ACNH files though on the acpatterns.com website, so you can just rename the file to .ACNH/.nhd and you will be able to import/dump and still have them work)

-------------------
## villager-exclusive items for import
Find the item file name below that you wish to work with (no links are mine) 
https://docs.google.com/spreadsheets/d/13d_LAJPlxMa_DubPTuirkIV4DERBMXbrWQsmSh8ReK4/edit#gid=951117189



### pink handbag
(pink handbag with flowers exclusive to villagers)
ToolBagFasionCute.Nin_NX_NVN.zs 

(item to be replaced)
BagBackpackSchoolbag0.Nin_NX_NVN.zs

1. import both files into toolbox
2. export the following individually from the wanted item:
- model
- materials
- textures
3. export model of item to replace and close toolbox
4. import both into blender (as individual collection to keep organized)
5. align wanted item as neccesary to align with replacement 
6. delete replacement item
7. export as uniquename.dae
8. open replacement item in toolbox
9. right click and replace the model with uniquename.dae
10. make sure to choose the material from the wanted item
11. ctrl+del all the files in the texture folder
12. right click and import textures
13. click on the material and on the right double click on each texture file and select the correct one (spm is mix file)(you may need to delete textures again and reimport in new window)
14. file - save as - replacedfilename.zs
15. copy into your atmosphere/contents/01006F8002326000/romFs/ folder and launch as normal


as suugested on toolbox: "I suggest converting the model's .dae file to fbx before importing into a tool like blender using autodesk fbx converter.
This is an issue specially with blender. Blender's dae importer is fairly buggy and fbx is much better supported."
https://www.autodesk.com/developer-network/platform-technologies/fbx-converter-archives

and 
from https://github.com/KillzXGaming/Switch-Toolbox/issues/514
1: export the model as dae and run it through fbx converter
2: export the animation as smd
3: install this plugin for blender
4: import the fbx then import the smd
https://developer.valvesoftware.com/wiki/Blender_Source_Tools







### cane
ToolCaneTtl.Nin_NX_NVN.zs







-------------------
(example used is casual chic dress-yellow, filename "TopsTexOnepieceAlongHCachecoeur0") 
TO IMPORT FROM SCRATCH/CHANGING MODELS

1. open/click+drag the following files to toolbox:
(make sure to render the file completely in the menu by opening each folder)

-Item file
> "\nxdumptool\Model\TopsTexOnepieceAlongHCachecoeur0.Nin_NX_NVN.zs"

NO MODEL INCLUDED - hence the "text" in the file name

mTops_Alb 

mTops_Mix 

mTops_Nm 

mTops_OP 

texture file type descriptions explained here
https://ac-modding.com/ACNH/mods/editing_textures

nice example of how these work
https://blenderartists.org/t/nrm-textures/551235

lots and lots of info about these file types here
https://www.youtube.com/watch?v=gUkY8ZoRfuQ&ab_channel=ThePassiveAggressor

helpful tutorial for acnh item modding
https://www.youtube.com/watch?v=677nQ-DQYQQ&ab_channel=RosieHorizons




-Item model (THIS IS SEPARATE FOR SOME CLOTHING TYPES) 
> "\nxdumptool\Model\PlayerBody.Nin_NX_NVN.zs"

textures are many separate files based on character customization


2. use .acnh or .nhpd 



'examples'

nrm files/ nrm maps
5 methods:
height map conversion
image renders
shape
hand drawn
3D software


