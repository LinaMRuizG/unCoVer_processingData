# Building databases for unCoVer projects
Here it is processed the daily databases published by the Instituto Nacional de Salud (INS) of Colombia. It is also used data from DANE. Theses data is the base of the unCoVer projects analysis.

## Description of files in this repository

- `scripts/` contains the codes used in the data processing
    -  `exploringDatosINS/` is a short exploration of the information published by the INS
    -  `trackingLocation/` tracks the column Location (Ubicación: UCI, hospital, casa, recuperado, fallecido) in each daily database published by the INS between March 15th 2020 and August 17th 2021
    -  `mergingLocation/` merges the matrices got in the tracking of the Location column for each case. After that, it is identified the cases going to hospital and/or ICU and with a defined outcome (i.e., recovery or deceased). Here is also made a first part of the hamornization for OPAL.
    -  `harmonizationOPAL/` those are different harmonization for OPAL. The first one is a continuation of the previous part.
    -  `buildingDatabases/` is the code used for built different databases for the analysis made in the proposals.
    -  `reviewingDataProcessing/` these review that the track made to the Location column is good.
- `dataOutput/` contains some of the outputs of the data processing codes
