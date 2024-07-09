# **BLOBIFIER - LITE**
## **For Voron 2.4 350mm only**

**This mod is specifically made for my setup. It may or may not work with your setup. Use it at your own risk. I will not make changes to accomodate your setup.** 

* My setup is as follow : 
  * Printer : Voron 2.4 350mm
  * ERCF 13 gates
  * Filametrix
  * Blobifier lite version
* My workflow is :
  * gates 0 to 9 have always the same filament (PLA black to white following the standard color code)
  * gates 10 to 12 have no dedicated filament. They can be anything depending what I need to print.
  * I use ERCF more as a color/filaùent selector than for multicolor print.
  * I often print the same gcode in different colors using the TTG function of HH.

* In this version of blobifer I don't use  :
   * the servo
   * the tray
   * the shaker
   * the blob counter
   * the initialize routine
   * the purge volumes from the slicer
 * I use
   *  a build in purge volume matrix build into the purge_volume.cfg file, the purge volumes are saved in mmu_vars.cfg
   *  the purge volume can e initialized manually or by copy/paste from a spreadsheet 
   *  a gate to gate filament instead of the from tool to tool purge volume
      *  This allow to print the same model in different color using the Happy Hare Tool To Gate mapping function.
   *  macro to adjust the purge volume any time, even during printing
   *  a gantry mounted brush and wiper based on this : https://www.thingiverse.com/thing:590448
* I make the blob directly on the bed of a Voron 2.4 350mm.
  * I use a ramp to get the blob out of the printer into an external bucket
  * STLs are made for my printer, there are no STL for other printers.








* Gantry mounted brush and wiper are based on : https://www.thingiverse.com/thing:590448


<p align=center><img src="Images/Ramp.JPG" width="350" alt="Ramp.JPG">
<p align=center><img src="Images/Bucket.JPG" width="350" alt="Bucket.JPG">
<p align=center><img src="Images/Brush.JPG" width="350" alt="Brush.JPG">

See the post on discord : https://discord.com/channels/460117602945990666/909743915475816458/1241678897649815625
