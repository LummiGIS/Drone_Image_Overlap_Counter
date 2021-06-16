# Drone_Image_Overlap_Counter
Creates a raster whos values are the number of image overlaps at that position.

Python 2.7

This script takes a feature class of polygons that represent the on-ground footprints of drone images (for example, the output of the image footprints script available from Agisoft  https://www.agisoft.com/forum/index.php?topic=2666.0) and creates a raster from those footprints.  This output raster’s pixel values are the sum of the overlapping image footprints.
This tool was written for ArcGIS 10.7 and requires an ESRI spatial analyst license in addition to the Arcpy library.
