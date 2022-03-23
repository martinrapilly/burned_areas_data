# burned_areas_data
Data used for the burned areas analysis made on the Dominican Republic on 2000-2020 MODIS images.

- burned_areas_reference_MODIS_2000_2020_DominicanRepublic.shp corresponds to burned areas polygons on pine and tropical humid forests detected on MODIS imagery in period 2000-2020 by photointerpretation and VIIRS hotspots visualization.
Photointerpretation of MODIS imagery has been made with 721 band combination (SWIR3/NIR/Red). The shapefile contains the date of a MODIS image previous to the event (img_inicio field) and following the event (img_final field); it also contains a rough estimation of confidence in the photointerpretation in percent, as estimated by the photointerpreter (conf field).
