# burned_areas_data
Data used for the burned areas analysis made on the Dominican Republic on 2000-2020 MODIS images.

- burned_areas_reference_MODIS_2000_2020_DominicanRepublic.shp corresponds to burned areas polygons on pine and tropical humid forests detected on MODIS imagery in period 2000-2020 by photointerpretation combined to VIIRS hotspots visualization.
Photointerpretation of MODIS imagery has been made with 721 band combination (SWIR3/NIR/Red). The shapefile contains the date of a MODIS image previous to the event (img_inicio field) and following the event (img_final field); it also contains a rough estimation of confidence in the photointerpretation in percent, as estimated by the photointerpreter (conf field).

- unburned_areas_reference_MODIS_2000_2020_DominicanRepublic.shp corresponds to unburned areas polygons on pine and tropical humid forests detected on MODIS imagery in period 2000-2020 by photointerpretation combined to VIIRS hotspots visualization.
Photointerpretation of MODIS imagery has been made with 721 band combination (SWIR3/NIR/Red). The shapefile contains the date of a MODIS image previous to the event (img_inicio field) and following the event (img_final field); it also contains a rough estimation of confidence in the photointerpretation in percent, as estimated by the photointerpreter (conf field).
The unburned areas have been delimited within the same periods and close to the same areas as those available in the burned areas reference product (mentioned above).

- burned_unburned_mean_values.csv contains the mean value of each burned and unburned polygon (wich contains x pixels inside of it) identified on MODIS imagery. It also contains the ratios of bands, the difference of NDVI, the NBR, dNBR and RdNBR indexes calculated on BURNED and on UNBURNED areas.
Here is description of each fields: 
POLYGON_BURNED: reference number of burned area polygons / BURNED_BEFOREB1 to BURNED_BEFOREB7: mean values of band x for one polygon before the fire / BURNED_AFTERB1 to BURNED_BEFOREB7: mean values of band x for one polygon after the fire / BURNEDratioB1 to BURNEDratioB7: ratio of Band x mean value before the fire on Band x mean value after the fire / BURNEDNDVIbefore: NDVI calculated on mean value before the fire / BURNEDNDVIafter: NDVI calculated on mean value after the fire / BURNEDdiffNetNDVI: rest between BURNEDNDVIbefore and BURNEDNDVIafter / BURNEDNBRbeforeWithSWIR3: NBR calculated on mean value before the fire / BURNEDNBRafterWithSWIR3: NBR calculated on mean value after the fire / BURNEDDNBRwithSWIR3: DNBR value / BURNEDRdNBRwithSWIR3: RdNBR value
The same scheme applies to UNBURNED fields. 
Altought there are exactly the same number of burned and unburned polygons, they do not cover the same areas; nevertheless, they do cover the same dates (for before and after fields).


