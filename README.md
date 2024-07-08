# **BLOBIFIER - LITE**
## **For Voron 2.4 350mm only**

* This version of blobifer don't use  :
   * the servo
   * the tray
   * the shaker
   * the blob counter
   * the initialize routine

* it make the blob directly on the bed of a Voron 2.4 350mm.
  * There are no STL for other printers.
* It work with from gate to gate instead of from tool to tool.
* It uses a saved purge volume matrix instead of the slicer one.
  * This allow to print the same model in different color using the Happy Hare Tool To Gate mapping function.
  * It is possible to adjust the purge volume while printing.
  * The start up array can be filled up with a macro that take the value from a matrix that can be set up with a spreadsheet.

