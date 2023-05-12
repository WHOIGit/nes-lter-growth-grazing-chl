## Creating a Data Package for NES-LTER Transect Cruise Plankton Growth and Grazing Data

This repository displays the workflow used to process the NES-LTER Transect cruise phytoplankton growth and microzooplankton grazing data in preparation for publication to the Environmental Data Initiative repository. This is an ongoing project, so we expect to update this package in the future as additional data are acquired.

This workflow includes the following:
1) cleans the provided data
2) performs quality assurance on the data
3) assembles and outputs the final XML file for submission to EDI

**Base Requirements:**
- Microsoft Excel
- R and R studio (*packages:* tidyverse, readxl, lubridate, devtools, EMLassemblyline, EML, maps, xml2)

### Collaborators:
Pierre Marrec (creator), Susan Menden-Deuer (principal investigator), Stace Beaulieu (associate; co-PI for the NES-LTER project), Jaxine Wolfe (associate; metadata provider)

### Package Status:
The first version of this data package is published to the EDI repository and can be found [here](https://portal.edirepository.org/nis/mapbrowse?scope=knb-lter-nes&identifier=5).
