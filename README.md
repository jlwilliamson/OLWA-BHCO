# Code for Williamson & Baumann, "Olive Warbler brood parasitism by the Brown-headed Cowbird and quantification of range overlap" [![DOI](https://zenodo.org/badge/306761721.svg)](https://zenodo.org/badge/latestdoi/306761721)

Paper *In Press*. 

Our observation of the second-documented instance of Olive Warbler brood parasitism by the Brown-headed Cowbird in New Mexico prompted us to ask: *How often do these two species co-occur synchronously and/or asynchronously in habitat and/or elevation?* To address locality overlap of these two species across the Olive Warbler range, we conducted a brief analysis of Global Biodiversity and Information Facility (GBIF) and eBird records. 

**Approach**: In this script, we use the 'rgbif' package to download GBIF records for the Olive Warbler (OLWA) and Brown-headed Cowbird (BHCO). Data were filtered and processed following the workflow outlined in our .rmd script file and described in our paper. We then imported OLWA and BHCO eBird records obtained from ebird.org and filtered these data by checklist effort. We merged filtered eBird data with GBIF data (to retain iNaturalist observations and data associated with vouchered museum specimens). Finally, we isolated localities of synchronous and asynchronous overlap between these two species, download and crop raster elevation layers to our study areas (Mexico and southwestern USA) and plotted asynchronous overlap localities, synchronous overlap localities, and documented parasitism events. 

Note: we opted *not* to use the elevation() function in 'rgbif' to pull missing elevation records, as this wasn't something we assessed in our paper. 

FYI, code in this script is not nearly as streamlined as it could be, but the code runs and it's fully annotated. Questions? Feel free to email me at williamson [at] unm.edu. 
