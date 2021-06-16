# Drone_Image_Overlap_Counter
Creates a raster whos values are the number of image overlaps at that position.

Version exist for ArcGIS (Python 2.7) and ArcGIS Pro (Python 3.x)

This script takes a feature class of polygons that represent the on-ground footprints of drone images (for example, the output of the image footprints script available from Agisoft  https://www.agisoft.com/forum/index.php?topic=2666.0) and creates a raster from those footprints.  This output raster’s pixel values are the sum of the overlapping image footprints.
These tools  requires an ESRI spatial analyst license and Agisoft Photoscan or Agisoft Metashape.

General Workflow:
Clone or download this repository.

Open your Agisoft Metashape project.

From Metashape go to Tools --> Run Script

Navigate to GetImageFootPrints.py and run with no parameters.

After the footprints are added to your Metashape project go to File --> Export ---> Export Shapes and save your shapefile.

From your favorite Python IDE open CreateImageOverlapCountFromAgisoftFootprintFilePy3.py

Set parameters to the input shapefile, an empty directory to store temp files, the path to the output image overlap count raster, and desired cell size.


