
***
# Introduction:
* 1 to 16 copper layers
* Board size up to 60 inches by 60 inches
* Uses English or metric units (i.e. mils or mm) for most functions.
* Footprint Wizard and Footprint Editor for creating or modifying footprints
* Import and automatic export of PADS-PCB lists
* Import and export to mechanical format DXF
* Import and export Pcad ASCII files
* Exports extended Gerber files (RS274X) and Excellon drill files
* Design rule checker
* Autosave

View
![PCB](https://raw.githubusercontent.com/Duxah/FreePCB/master/pictures/img2.png)

***
# About development
The FreePcb-2.000 and above program presented on this site is an upgrade of version [1.359](www.freepcb.com) published in 2010. Now FreePcb has made great strides in comparison with the 2010 version and is suitable for both simple and large-scale developments, although the appearance remains the same. Includes footprint editor, provides the ability to create your own libraries, can import external netlists in the PADS-PCB format, supports the preservation of REF-names of parts when paneling printed circuit boards. The program is focused on accessibility, ease of use, saving computer hard disk memory, but at the same time it includes almost all the tools necessary for professional use. A distinctive feature of this program is the interface with the use of function keys, which speeds up the process of editing a printed circuit board for an experienced user. Start working with FreePCB right now to appreciate all benefits of this interface. 

(Translated from Russian by Google inc.)

***
# Major improvements and new features
* Improved graphical display of selected objects
* Improved detailing frame
* free rotation of parts
* [moving the group to the opposite side](https://youtu.be/WTI2HnneCzk)
* set of zero coordinate on any object(menu TOOLS)
* [merge a group of parts into one object](https://youtu.be/ef0Bef-Ql0M)
* [alignment of parts](https://youtu.be/5YJZ7ADQruM)
* [alignment of traces](https://youtu.be/Sb_mCNirUw4)
* [alignment of mergers](https://youtu.be/dCAhdzjO4l8)
* Improved work with polygons
* the ability to set a specified gap between any lines [(set_clearance)](https://youtu.be/Z1GgYGOtFfU)
* preparation of the code for the introduction of micro transition holes
* possibility of rounding vertices of traces
* possibility of adding drop vias (using the external application RoundingRect.exe)
* replacing some parameters in the project file using the external program Replace.exe
* combining several footprints into one directly in PCB editing mode using the external program Libraries.exe
* the ability to organize libraries alphabetically, by the number of pins or by the number of holes (Libraries.exe)
* external program [infobox.exe](https://youtu.be/I0mb6RNXuqo) knows how to [find parts](https://youtu.be/8IQnL1ws65g) on a printed circuit board
* in freepcb, you can not fill copper polygons. gaps are drawn automatically when creating the Gerber files, but sometimes you need to fill it. External program [AREA_SPLITTER.EXE](https://youtu.be/2jqGSPgFSpU) fills polygons
* [export to mechanical format dxf](https://youtu.be/5NpD_ZXCbkI)
* import from dxf
* [import pictures from bmp](https://youtu.be/WMQjF043Kko)
* [Export to commercial PCAD (ACCEL ASCII)](https://youtu.be/G5TM_Og5mOk)(There is a nuance that the origin should be in the lower left corner outside the circuit board elements.)
* Import PCAD( ACCEL ASCII )
(2014-2017)

`Version 2-019 (2018-02-20):`

* The function of automatic [selection of parallel segments](https://youtu.be/5JjDa58_ABA) for quick editing is added 
* AREA_SPLITTER.EXE and [INFOBOX.EXE improved](https://youtu.be/ItGi7xaLnlY), [show pins](https://youtu.be/_XKBCJiFBmQ).

`Version 2-020 (2018-05-01):`

* added 3 new layers:  2 for notes, scribing
* when moving the origin in the footprint the position of the part on the board remains
* when selecting a detail pin, the network is also highlighted
* in export DXF_3dFaces drawing of pads by solid
* [in InfoBox when clicking on a cell in the column "Net in PCB" on the left all pins of this net are displayed](https://youtu.be/2NqhzvQQsBQ)
* [in InfoBox when clicking on a cell in the "Pin" column on the right all pins of this detail are displayed](https://youtu.be/2NqhzvQQsBQ)
* [Select/Unselect](https://youtu.be/4FUoShPmiI8)

`Version 2-021 (2018-06-01):`

* in the InfoBox column is added the [range of indexes](https://youtu.be/9mD0dIe6yyk) of notation details
* added the SET ORIGIN TO SELECTED ITEM function in the TOOLS menu
* two grid styles: points and lines
* Improved auto-refs (REF-AUTO-POS)
* added the SHOW_MERGES (F6) button to find the merge on the board, [selection several mergers](https://youtu.be/z-ttbtUvRCA)

`Version 2-022 (2018-07-22):`
 
* added the SELECT ALL button in the EDIT menu

`Version 2-023 (2018-10-07):`

* in the footprint editor added the ability to create pins with one common name (MULTIPIN)
* added the ability to divide the net into 2 different (SPLITNET)
* added the ability to block a netlist in the Project-> Nets menu ...

`Version 2-024 (2018-12-31):`

* added a button to select all objects located inside any polyline (F9 INSIDE CONTOUR)
* copper polygon with edge thickness 0 and the none fill style is now a ghost polygon, and serves as a fill area for the program Area Splitter
* rotation of a group of objects at any integer angle
* if the symbol `|` is added to the element designation (REF) that the text after the symbol on the printed circuit board is not displayed (for multichannel devices).
* display of clearance when the trace segment moves by the keyboard arrows (set in the TOOLS->DRC->trace to trace, you can temporarily change it with the SET_CLEARANCE function, return to the initial value when you save the file again).

`Version 2-025 (2019-04-12):`

The SET_CLEARANCE function becomes universal and takes on a larger scale. For example, you can set clearance between the segment of trace and the side of copper area.
* the measurement tool (activated with the M key) leaves a trace on the screen with the display of numerical value, and is a polyline, i.e. allows you to measure the perimeter of a polygon
* Opening a file by dragging on the window

`Version 2-026 (2019-04-19):`

* Added option to the LAYERS menu: file colors versus system colors.

`Version 2-027 (2019-04-27):`

* [Improved SET_POSITION](https://youtu.be/7WguD56Wu3U) function for polyline vertices 

`Version 2-028 (2019-06-12):`

* In the footprint editor, you can edit a group of objects: duplication, rotation, mirroring.
* Added warning in DRC check if PCB name is missing
* When you press the buttons 3 or 4 again, the silk screen layer goes to the background
* Now you can move the side of the polyline with the keyboard arrows
* A button to quickly [export gerber files to ViewMate](https://youtu.be/ZzjedfBTwvc) has been added to the File menu. (for viewing and printing)
* Overwrite protection when saving a file that was created in FREEPCB version 1.359
* Specifying a folder with FREEPCB projects in the INFOBOX SETTINGS menu is no longer required (21.06.2019)

![](https://raw.githubusercontent.com/Duxah/FreePCB/master/pictures/cloud-down.png) The [download](https://drive.google.com/open?id=1qPDMzfwV7oMmpA2gsspwId4ZLeLsT6BZ) (Updated 27.06.2019!) includes a folder with the program, manual 1.359, footprint libraries, examples of printed circuit boards, a description of the 2.028 file format for developers.


![](https://raw.githubusercontent.com/Duxah/FreePCB/master/pictures/По%20рукам.png) If you like version 2-028, place a `freepcb.dev` link on your site. Have fun using FreePcb

***

[More video:](https://www.youtube.com/watch?v=BqJPxMCFzyc&list=UUAfxUv-ywajGqFkucOYEtbw)
* [Routing branch](https://youtu.be/FPJLVRgZ5So)
* [Remove bridge](https://youtu.be/aCoLDw9o3DA)
* [Arc elements](https://youtu.be/Rl8hyAXn1Lk)
* [Align merges](https://youtu.be/dCAhdzjO4l8)
* [Align parts](https://youtu.be/5YJZ7ADQruM)
* [Align board](https://youtu.be/2pZpUzymLcc)
* [Drag part](https://youtu.be/36UT71BUEm0)
* [Hilite 2 gerber](https://youtu.be/2q5XgN500uE)
* [Hilite first pin and printing](https://youtu.be/gYQWfOK9_QI)
* Example routing
* Example routing with external netlist
* Export DXF example
* [Copper area cutter](https://youtu.be/rhsPvqH7rdo)
* [Copper area cutter](https://youtu.be/DLLKXDGEXuA)
* Copper area cutter
* [Import BMP](https://youtu.be/WMQjF043Kko)
* [Combine footprints](https://youtu.be/4xpSpHkO-iM)
* [Save footprint to library](https://youtu.be/SL4raX00w2g)
* [Editing traces](https://youtu.be/CZk4pxCQKaQ)
* [Change side](https://youtu.be/WTI2HnneCzk)(for group)
* [Set Clearance more](https://youtu.be/f3_C0MA4M1Q)
* [Split Net](https://youtu.be/gE-gt-o9I4Y)
* [Set Ref & Value size](https://youtu.be/HjpzUJ0DZh0)(for group)
* [Radius of trace to raise/lower](https://youtu.be/BqJPxMCFzyc)
* How to save designations when panelizing
* 1  way
* [2 way](https://youtu.be/YiW7-XE1Sa0)
* How to save footprints when paneling if the footprint names in files are the same, but footprints are different

***
Contacts.
* [User forum](https://groups.yahoo.com/neo/groups/FreePCB/info) on Yahoo Group. 
* If you have any suggestions related to FREEPCB or you do not want to submit your question for public review, send an [email](mailto:freepcb.development@gmail.com).
* If you want to improve the translation of this document send your file to [email](mailto:freepcb.development@gmail.com)

***
`useful links`
1. License
2. FreePcb user guide 1-359
3. FreePcb "How to.." guide
4. File format 2-028 with comments
***
# Get started with FreePcb
Download the folder with the application and run the file FreePcb.exe

## Training on the example of the smart_kitchen.fpc file in the EXAMPLES folder
In this example, 3 independent circuit boards. (this is called a printed circuit board panel). In the context menu of the right mouse button, click the full view to see them entirely.

`this repository is under development` ©2019
