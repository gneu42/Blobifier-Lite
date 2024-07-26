**PRINTER_VAR and PRE_LOAD macros to insert in your macro file**

These macros ensures that the first filament load of the print is done at BLOBIFIER_PARK position.


[gcode_macro PRINTER_VAR]

variable_first_load:     1 #used for the first load at print start : 1= First load done

gcode:


[gcode_macro PRE_LOAD]
gcode:
   {% set fl = printer['gcode_macro PRINTER_VAR']['first_load']|int %}
   {% if fl == 0 %}
     BLOBIFIER_PARK
   {% endif %}


**You must add :** 

	 SET_GCODE_VARIABLE MACRO=PRINTER_VAR VARIABLE=first_load VALUE=0 

at the start of your PRINT_START macro, and 

	SET_GCODE_VARIABLE MACRO=PRINTER_VAR VARIABLE=first_load VALUE=1

after the filament has been loaded.

You can also add those line in other macro as needed.