# NCF
National Channel Framework

Original source data from USACE can be found here:

<https://geospatial-usace.opendata.arcgis.com/datasets/9227967a2748410983352b501c0c7b39?layer=2>

Downloads are available in kml, shp, gdb, or csv formats

Note: shapefiles are annoying and cut off field names to 10 characters, so the geojson provided here might be more useful

## Changelog
3/8/2021
### Lower Miss
- Corrected and appended MILEAGESTART and MILEAGEEND for all reaches
- Overlaps from mile 319-347: Remove CEMVK_LM_01_GCB_1 and all BH reaches except CEMVN_MS_04_BH4_01. Keep CEMVK_LM_01_GCB_2 onwards
- Overlaps from mile 623-645: Keep OVL reaches, remove CLD reaches
- Fix gap between GCB_8 and GCB_9 by extending GCB_9 to meet the end of GCB_8
- Fix gap between CVB_1 and CVB_2 by extending CVB_2 to meet the end of CVB_1

### Upper Miss
- Reshaped EPC_1 so that it starts where HIK_38 ends on the lower Miss
- Appended mile markers for all reaches

### Ohio
- Appended mile markers for all reaches
- Reshaped CAI_1 so that it starts where HIK_38 ends on the lower Miss

## To Do
### Lower Miss
- Fix missing or misshapen channel reaches on the Lower Miss from Baton Rouge to the Gulf
- Deal with duplicate reaches (FRI_41 to 43) - possibly combine into a single reach

### Ohio
- Fix duplicate/separated reaches like WIO_9, WIO_10 and WIO_29

### General items
- Find and combine or remove reaches with identical channelreachidpk keys (often occurs when reach is across an island)

