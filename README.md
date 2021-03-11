# NCF
National Channel Framework

Original source data from USACE can be found here:

<https://geospatial-usace.opendata.arcgis.com/datasets/9227967a2748410983352b501c0c7b39?layer=2>

Downloads are available in kml, shp, gdb, or csv formats

Note: shapefiles cut off field names to 10 characters, so the geojson provided here might be more useful

## Changelog
### 3/10/2021
- Combined duplicate/split reaches into a single reach. Includes:  
CELRH_KA_HD_WIN_26  
CELRH_OH_HD_BEL_17  
CELRH_OH_HD_BEL_18  
CELRH_OH_HD_BEL_29  
CELRH_OH_HD_BEL_35  
CELRH_OH_HD_BEL_36  
CELRH_OH_HD_WIO_10  
CELRH_OH_HD_WIO_29  
CELRH_OH_HD_WIO_9  
CEMVM_LM_18_FRI_41  
CEMVM_LM_18_FRI_42  
CEMVM_LM_18_FRI_43  
CENAB_MD_10_10K_1  
CENAB_MD_26_026_1  
CENAB_MD_68_GR1_1  
CENAB_MD_71_109_1  
CENAB_MD_72_110_1  
CENAE_NH_02_PIS_1  
CENAE_NH_02_PIS_2  
CENAE_NH_02_PIS_3  
CENAE_NH_02_PIS_5  
CENAE_NH_02_PIS_6  
CENAE_NH_02_PIS_7  
CENAE_NH_07_LIT_1  
CENAE_NH_07_LIT_3  
CESAC_GT_01_GTH_14  
CESAM_PH_05_PUS_1  

### 3/8/2021
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

### General items
- Deal with duplicate river miles on river forks
- Resize or reshape channel reaches in coastal areas

