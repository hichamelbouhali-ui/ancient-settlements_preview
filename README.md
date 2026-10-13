# ATTENTION: This repository currently contains the database schema, data dictionary, and preview layers. The complete GeoPackage (.gpkg) will be made publicly available upon publication of the related data paper.

[DOI:](xxx)

This readme file was generated on 2026-10-09 by Hicham El Bouhali. This README uses a template provided by the [CORNELL DATA SERVICES](https://data.research.cornell.edu/data-management/sharing/readme/). 


## **Rise and Fall of the Assyrian Empire: Archaeological Settlements of the Syrian-Iraqi Jazīra from the Middle Bronze Age to the Iron Age.**

<img width="800" height="612" alt="archaeological surveys and sites used for the dataset" src="https://github.com/user-attachments/assets/68400f9a-4ef6-4f65-acb3-3023f53dc22c" />

Figure 1. Map showing archaeological surveys and sites used for the dataset. © Created by Hicham El Bouhali with QGIS 3.44.15. 


**Author/Data Curator and Maintainer**:

- Name: Hicham El Bouhali
- ORCID: [0009-0008-2899-6715](https://orcid.org/0009-0008-2899-6715)
- Institution: Kiel University, Institute for Prehistoric and Protohistoric Archaeology - Exzellenzcluster ROOTS 
- Address: Leibnizstrasse 3, 24118 Kiel, Germany
- Email: helbouhali@roots.uni-kiel.de

**Author/Associate, Principal Investigator and Grant Holder**:

- Name: Alessio Palmisano
- ORCID: [0000-0003-0758-5032](https://orcid.org/0000-0003-0758-5032)
- Institution: University of Turin, Department of Historical Studies
- Address: Via Sant'Ottavio 20, 10124 Turin, Italy
- Email: alessio.palmisano@unito.it


**Date of data collection**: 2024-09 to 2025-10

**Geographic location of data collection**: 

- Region: Syrian-Iraqi Jazīra
- Geographic Coordinate System: EPSG:4326 - WGS 84
- Northern boundary: 37.162932837 (decimal degrees).
- Southern boundary: 34.196878735.
- Eastern boundary:  43.651270479.
- Western boundary:  37.681681208.

**Information about funding sources that supported the collection of the data**:

- This project is part of the  part of the Italian Ministry of University and Research (MUR) funded “The Empire Strikes Back: The Geography of Governance in the Assyrian Empire” project. 


# SHARING/ACCESS INFORMATION

**Licenses/restrictions placed on the data**: [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/)

**Links to publications that cite or use the data**: 

**Links to other publicly accessible locations of the data**: The dataset is openly available in the Zenodo depository at the following link: 

**Data origin**: Secondary and Processed data from originally published materials (see "References.txt" file).

**Recommended citation for this dataset**: Appropriate citation will be provided once the data paper is published.


# DATA & FILE OVERVIEW

### File List:

- **dataset** folder:
  - **SyrianIraqiJazīra** - a geopackage (.gpkg) database containing three layers:
      - **StudyArea** - a polygon layer (.shp) delimiting the spatial extent of the study area in which the sites were chosen for the dataset. 
      - **ArchaeologicalSurveys** - a polygon layer (.shp) showing the spatial extent of all the archaeological surveys used. 
      - **ArchaeologicalSites**- a point layer (.shp) of the sites in Syrian-Iraqi Jazīra.
  - **ArchaeologicalSites** - a spreadsheet ".csv" of the sites in Syrian-Iraqi Jazīra.
  - **METADATA** - a ".txt" file which contains data and field description of the spreadsheet.
  - **References** - a ".txt" file containing a comprehensive list of all the references from which the data have been collected.


**Relationship between files**:

- **METADATA.txt** contains information about the attributes of the archaeological surveys and archaeological sites in the geopackage database.


# METHODOLOGICAL INFORMATION 

### Methods for processing the data: 
- Digitalization of archaeological surveys and sites from published materials.
- Chronological harmonization of the source data.
- In QGIS: standardization of data in a geopackage database with each site-phase represented by a point geometry, and digitalization of archaeological surveys in a polygon geometry.


### Instrument or software-specific information needed to interpret the data: 

- GIS software to visualize the geopackage database: [QGIS](https://qgis.org/) is a recommended free, open-source and multi-platform software for this purpose. Data was generated using QGIS 3.34 and higher. Some visualization features may not work properly with older versions of QGIS. 


*Standards and calibration information*: 

- Chronological Framework for the Syrian-Iraqi Jazīra used in the dataset (see the data paper for more information).


|Period	               |Historical Period     	 | Start Date (BC) | End Date (BC) |
|----------------------|-------------------------|-----------------|---------------|
| Early Bronze Age IV	 |           ---           |      2300	     |      2000     |
| Middle Bronze Age I	 | Old Babylonian / Khabur |      2000	     |      1800     |
| Middle Bronze Age II | Old Babylonian / Khabur |	    1800	     |      1600     |
| Late Bronze Age I	   |          Khabur	       |      1600	     |      1500     |
| Late Bronze Age I	   |        Mitannian	       |      1500	     |      1400     |
| Late Bronze Age II	 |        Mitannian	       |      1400	     |      1300     |
| Late Bronze Age II	 |      Middle-Assyrian	   |      1300	     |      1200     |
| Iron Age I	         |      Middle-Assyrian	   |      1200	     |      1000     |
| Iron Age II	         |      Middle-Assyrian	   |      1000	     |       900     |
| Iron Age II	         |        Neo-Assyrian	   |       900	     |       800     |
| Iron Age III	       |        Neo-Assyrian	   |       800	     |       600     |
| Iron Age III	       |       Post-Assyrian	   |       600	     |       550     |
| Iron Age III	       |           ---           |       550	     |       330     |


### Quality-assurance procedures performed on the data:

- All data have been checked and standardized.
- Estimated site sizes have been refined by using multiple sources, wherever possible (archaeological surveys, excavation reports, etc.)
- Site locations have been cross-checked with multiple sources (see above) and refined by using satellite imagery, topographic maps, and other published materials.

### People involved with sample collection, processing, analysis and/or submission: 

- Hicham El Bouhali

# DATA-SPECIFIC INFORMATION FOR: SyrianIraqiJazira.gpkg - ArchaeologicalSites.shp / ArchaeologicalSites.csv

**Number of fields**: 17

**Number of cases/rows**: 1,996

**Fields lists and descriptions**:

- Id (integer): unique identifier of the archaeological site.
- Id_Phase (integer): unique indentifier of a particular site-phase. 
- Toponyms (string): modern name of the archaeological site.
- Ancient Toponyms (string): ancient name of the archaeological site (if available).
- Type (string): typology of archaeological site (settlement - fort - temporary camp).
- Period (string): the archaeological period to which each site-phase belongs.
- Historical Period (string): the historical period to which each site-phase belongs.
- StartDate (integer): approximate start date for the occupation of a site-phase, expressed in absolute calendric years. 
- EndDate (integer): approximate end date for the occupation a site-phase, expressed in absolute calendric years.
- Longitude (decimal): Geographic/Unprojected WGS84 eastings.
- Latitude (decimal): Geographic/Unprojected WGS84 northings.
- LocQual (string): degree of accuracy of the point representing the site.
- SizeHA (integer): estimated site size for each site-phase.
- SizeQual (string): degree of the accuracy of the estimated site size for each site-phase.
- Source (string): bibliographic reference(s) from which the archaeological data have been collected. 
- Source_id (string): unique identifier of the archaeological site in the original source(s).
- Comments (string): supplementary information.

