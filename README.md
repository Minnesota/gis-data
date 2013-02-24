gis-data
========



Sources and Links
-----------------

- http://www.mngeo.state.mn.us/chouse/data.html
- http://www.mngeo.state.mn.us/chouse/wms/index.html
- http://deli.dnr.state.mn.us/data_catalog.html
- http://gdwweb1.ftw.nrcs.usda.gov/
- http://www.mngeo.state.mn.us/chouse/metalong.html
- http://geo.data.gov/geoportal/catalog/main/home.page
- http://www.datafinder.org/catalog/index.asp
- http://www.gis.leg.mn/html/download.html
- http://www.dot.state.mn.us/maps/index.html
- http://data.dot.state.mn.us/datatools/
- http://www.dot.state.mn.us/maps/gisbase/html/datafiles.html
- http://deli.dnr.state.mn.us/other_data_sources.html
- http://www.umesc.usgs.gov/states/m/mn_gis_data.html
- http://www.mngeo.state.mn.us/GeoServiceFinder/
- http://www.mngeo.state.mn.us/chouse/wms/wms_image_server_layers.html
- ftp://nhdftp.usgs.gov/DataSets/Staged/States/FileGDB/HighResolution/

Additional Data Formats
-----------------------

Some of this data is only available as Esri Shapefiles. Should you need to
convert to KML, and don't want to spend time Googling. This approach assumes
familiarity with a command line.

 1. Install [GDAL](http://www.gdal.org/). Since there are a number of
    dependencies (proj4, et al.), it is easiest to use a package manager. 
    * Homebrew: `brew install gdal`.
 2. Make sure `ogr2ogr` is now in your path.
 3. Run the command: `ogr2ogr -f KML output.kml input.shp`, substituting the
    path names to the relevant files.

`ogr2ogr` will convert a variety of other filetypes as well. 
