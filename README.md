# vrcloset
## wip resource for modding wearables in Animal Crossing: New Horizons
don't expect too much here for a while, it's literally just messy notes full of typos and formatting errors for now


no models for clothing? understandable. these items work just like the custom code clothing does in-game
these clothing types use a separate model because they are shared
models for accessories, shoes, hats etc. will be included in the item file because they are unique


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
Find the item file name below that you wish to work with (no links are mine) 
https://docs.google.com/spreadsheets/d/13d_LAJPlxMa_DubPTuirkIV4DERBMXbrWQsmSh8ReK4/edit#gid=951117189
(example used is casual chic dress-yellow, filename "TopsTexOnepieceAlongHCachecoeur0") 




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
