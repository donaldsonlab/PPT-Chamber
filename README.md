# Partner Preference Test Chamber

This repository contains 3D models, created in Solidworks, and fabrication files for designing and constructing a Partner Preference Test (PPT) chamber. This is divided into three
sections, two of which provide mounting holes to tether animals. When not in use, the tether holes and slots on the sides may be covered up by a clip-on hole cover. This cover
can slide from the slot to the hole, covering one at a time.

![alt text](images/PPT.JPG)

The walls of this chamber are laser cut out of clear 3/16" acrylic sheets, painted matte white where needed, and assembled using plastic cement. The files used on the laser 
cutters are located in the [DXF}(dxf) directory. To optimize the nesting of parts on as few acrylic sheets as possible, we use an open source software called 
[Deepnest](https://deepnest.io/). We 3D print the hole cover clips on a Zortrax M200 Plus FDM printer with PLA, ABS, or Z-ULTRAT filament. The .STL file for this is in the 
[STL}(STL) folder along with a [PPT_cornerBracket](PPT_cornerBracket.STL) file, which is just used to hold the corners of the chamber together while glueing.


       Bill of Materials      
--------------------------------
|Part|Description|Quantity|
-----|------------|-------|
PPT_Floor             |Laser cut [PPT_Floor.dxf](/DXF/PPT_Floor.dxf)|1|
PPT_LongWall          |Laser cut [PPT_LongWall.dxf](/DXF/PPT_LongWall.dxf)|2|
PPT_SideWall          |Laser cut [PPT_SideWall.dxf](/DXF/PPT_SideWall.dxf)|2|
PPT_InsertGuide_Large |Laser cut [PPT_InsertGuide_Large.dxf](/DXF/PPT_InsertGuide_Large.dxf)|4|
PPT_InsertGuide_Small |Laser cut [PPT_InsertGuide_Small.dxf](/DXF/PPT_InsertGuide_Small.dxf)|4|
PPT_HoleCover         |Laser cut [PPT_HoleCover.DXF](/DXF/PPT_HoleCover.DXF)|2|
PPT_HoleCover_Clip    |3D printed PLA/ABS [PPT_HoleCover_Clip.stl](/STL/PPT_HoleCover_Clip.stl)|2|
Plastic Cement        |Plastruct Plastic Weld or IPS Weld-On 3 Acrylic Plastic Cement|<1|
Matte White Paint     |[Krylon Fusion All-In-One Spray Paint, Matte, White, 12 oz.](https://www.walmart.com/ip/Krylon-Fusion-All-In-One-Spray-Paint-Matte-White-12-oz/678882687)|<1|

The brand of acrylic cement is not important, as long as it can hold the acrylic pieces together. Similarly, the brand of paint is unimportant and can either be *matte* or *flat*, although matte finishes can typically withstand more cleaning.

**Note:** If the wall 
thickness is adjusted, the 3D models and .DXF files must also be modified. This can be done in the text file, [PPTequations.txt](PPTequations.txt), which contains equations
used for each Solidworks part. Simply change the "WallThickness" and/or "FloorThickness" to the desired value and rebuild or refresh the part file. This can also be done with the
other variables in PPTequations.txt if wanting to modify the width, height, or depth of the PPT chamber.

