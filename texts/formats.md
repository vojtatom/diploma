# Formats
List of formats 

Based on the analysis bellow, there are 4 main classes of used formats:
* ArcGis outputs: DBF + SHP + PRJ
* CityGML or CityJSON
* GeoJson
* DGN or DWG

+ https://www.koncepcebim.cz/koncepce

---
## 3D models 

The available 3D models can be conceptually divided into three catheories - either we talk about buildings, briges or other human-made features, then there are trees and flora in general, and the last cathegory is the terrain.

### Buildings, bridges + other features
As the ArcGis is one of the comertional used softwares, the usual outputs are documented here: https://gisgeography.com/arcgis-shapefile-files-types-extensions/

 * DBF - attributes and IDs
 * SHP - spatial vector data
 * SHX - indices (Esri + AutoCAD based)


 * PRJ - metadata - coordinate system, projection, center looks like project shorter metadata
 * CPG - encoding, UTF8
 * SBN + SBX - make up a shape index to speed up spatial queries, looks like binary or unknown encoding
 * SHP.XML ?? looks like duplicite info from other files
 * XML - more info about projection, coordinate systems, shapefile metadata, system paths

or possibly all in one (minus the info for queries acceleration): 
* GML - https://www.ogc.org/standards/citygml 

Other available information in a separate form is the 
* number of building floors (CSV + SHP)
* how's the land currently used [současný stav využití území] (DXF, GML, SHP) + CSV
* price map of the land (GML, SHP)

### Terrain
* DGN
* DWG
* polygonZ - after extract looks like the list of files from arcgis above
* TIFF as raster

DGN and DWG are alternatives, each proprietary. DGN is developed by Bentley Systems, MicroStation and Intergraph's Interactive Graphics Design System (IGDS) CAD programs, DWG is develped by Autodesk. **Both are vector formats,** not easily parsable:

* https://github.com/rurban/dgnlib
* http://dgnlib.maptools.org/
* https://gdal.org/ loading raster and vector formats, c++ and python api, a lot of approximations

### Flora
??? Could not find much info about that...


## City Structure Elements + Networks + Community waste disposal + Culture
* GML - I tried to modify the data for Prague into GeoJson format but there was a problem with the XML (wrong ID or something)
* DXF - Autodesk
* SHP + DBF + PRJ - ArcGis (Probably an old classic of files for geospatial data?)
* occasionally also GeoJSON

The actual data conists of:
* technical map (netowrks, netowrk access points)
* building areas + "technické využití území"
* územní plán (?) - public service buildings (points, lines, areas), the use of the land, planned changes

## Transport
Trajectories with metadata, information about streets, public transport, bicycle roads, and parking spots.  

* GML
* GeoJSON
* DXF
* SHP

There is additional data in CSV (possible issue with key mismatches between spatial data and csv).

## Geology
Radon + stability of the ground, formats GML, GeoJSON, DXF, SHP.

## Noise
Noise map **is available for both day and night** in DXF, GML, SHP.

* noise map in general
* noise map for transport
* noise-canceling elements (walls, barriers) (also in GeoJSON)


---
