# Sample Collection

At each station, hydrographic data of depth and temperature were collected with an SBE911 (Seabird Electronics Inc.) CTD-rosette system. Seawater for the experiments was collected using multiple Niskin bottles and sometimes from different CTD casts at a given location. Cast and bottle numbers are reported in the data table. Depth and temperature values of the seawater collected for the experiments reported in the data table are averaged from bottle summary files produced with Seabird software onboard ship and have not been corrected for salts.

# Experimental Set-Up

Rates of phytoplankton growth and microzooplankton grazing were quantified using a 2-point modification of the dilution method (Morison and Menden-Deuer, 2017). Whole seawater (WSW) was gently transferred from a Niskin to a 10-L polycarbonate carboy through a 200-µm mesh to remove mesozooplankton predators (e.g. copepods).

Diluent was prepared by gravity filtration through a 0.2-µm membrane filter capsule (PALL) from the Niskin to the carboys. The appropriate amount of WSW was added to the filtered water to obtain an approximate 20 percent WSW dilution (20WSW). The effective dilution level was calculated from the ratio of the initial chlorophyll-a (chl-a) concentration in the 20WSW diluted treatment to the initial chl-a concentration in the WSW treatment. The carboys were light-protected by black plastic bags and gently mixed while water was siphoned into duplicate 1.2-L clear polycarbonate bottles. To ensure the gross growth rate of the phytoplankton was not nutrient limited, a central assumption of the dilution method (Landry and Hasset, 1982), incubation bottles were amended with macronutrients (10 µM SiO4, 10 µM NO3, 1 µM PO4). An additional set of WSW bottles without additional nutrients was added to assess nutrient limitation or toxicity effects. For each dilution (20WSW and WSW), nutrient treatment (nutrient amended and without nutrient), and light treatment (as percent of available light, see below), incubation bottles were collected in duplicate (in triplicate on cruise EN687, summer 2022).

Bottles were incubated for 24 h in clear, deck-board, flow-through, 1-m^3 incubators. During some cruises, surface water was incubated at different light levels to simulate the contrasting light conditions (e.g. sunny/cloudy weather, well-mixed/stratified water column) under which phytoplankton could be growing in the surface ocean and to study the effect of light on phytoplankton growth and microzooplankton grazing rates. Due to persistent lack of differences in growth as a function of the two light levels, the light treatment was omitted in later cruises. Beginning with cruise EN668 (summer 2021), surface water was incubated only at a 65 percent light level, which simulated the in situ light conditions. Water sampled at deeper depths (not surface) was incubated at lower light levels, which simulated the light conditions at these depths. Neutral density screen bags were used to create the different light treatments. The incubators were free of overhead obstructions to avoid shading during the day and covered by a tarp at night to minimize light pollution from deck lighting. Natural movement of the ship kept the bottles in the incubators agitated over the incubation period. Temperature within the incubators was maintained equivalent to surface temperature through continuous flow-through from the ship's seawater system. Beginning with cruise EN655 (summer 2020), chillers were used in some tanks to get better temperature control during the incubation and to better reproduce the temperature conditions observed at deeper depths. Temperature and light in the incubators were monitored at 5-minute intervals with HOBO (Onset) data loggers. Temperature (°C) and light (lux) measurements recorded during each of the incubation experiments are available in .csv files in the data package other entity .zip file, with the naming convention "CRUISE\_temp\_inc\_X.csv" where CRUISE is the cruise name and X is incubator number.

# Phytoplankton Growth and Protist Grazing Rate Estimates

Initial (T0) chlorophyll-a (chl-a) concentration was determined from triplicate 120-150 mL subsamples from carboys used to fill incubation bottles. Final chl-a concentration (TF) was determined from triplicate 120-150 mL subsamples from bottles after the 24 h incubation. The extraction method followed Graff and Rynearson (2011) except here we used 95 percent ethanol as a solvent (Jespersen and Christoffersen, 1987). Extracted chl-a concentration was determined using a Turner AU10 fluorometer after a 12-h extraction period at room temperature. In addition, the size structure of the initial phytoplankton community was characterized from T0 triplicate size-fractionated chl-a samples (greater than 0.7 µm (GF/F) and greater than 10 µm). At TF, size-fractionated chl-a concentration at 10 µm were also measured for 20WSW, WSW without nutrient addition and WSW nutrient-amended bottles. During the two 2018 cruises (EN608 and EN617) and during the winter 2019 cruise (EN627), size fractionation at 10 µm was performed only on nutrient-amended samples.

Phytoplankton growth rates and protist grazing rates were estimated from changes in chl-a concentration over the 24 h incubation. For each incubation bottle, the apparent growth rates (k, 1/d) were calculated as:

k=1⁄t×ln(C\_t⁄C\_0)

where t is the incubation time (d) and C\_t and C\_0 the final and initial chl-a concentration (mg/m^3), respectively.

Protist grazing rates (g, 1/d; column 'grazing' in the product data table) were estimated with the equation:

g=(k\_d-k\_N)⁄(1-x)

where k\_d and k\_N are the apparent growth rates in 20WSW and WSW nutrient-amended treatments, respectively, and x is the achieved fraction of WSW in the diluted treatment calculated from T0 chl-a in 20WSW and WSW (Landry et al., 1984). Accordingly, the instantaneous, or in situ, growth rate (mu\_0, 1/d) was estimated (as in Landry et al., 2008):

mu\_0=g+k\_NoN

where k\_NoN is apparent phytoplankton growth rate k without nutrient addition.

The potential for nutrient limitation was assessed by comparing apparent phytoplankton growth rate k in nutrient-amended (k\_N) and nonamended (k\_NoN) replicates using a paired t-test. If a significant difference was found (p below 0.05) between k\_N and k\_NoN, nutrient-amended growth rates (mu\_N, 1/d) were also calculated as mu\_N = g + k\_N. Otherwise, all k\_N and k\_NoN triplicate of replicate values were used to calculate both g and mu\_0.

Since size fractionation at 10 µm was performed only on nutrient-amended samples during cruises EN608, EN617, and EN627, growth rates reported on greater than 10 µm and less than 10 µm fractions in this study were nutrient-amended growth rates (mu\_N) when nutrient limitation was observed. If no nutrient limitation was observed, mu\_N obtained is equivalent to mu\_0.

The uncertainty of g was quantified from the mean standard deviation of k\_dil, k\_NoN, and k\_N. Grazing rate (g) was set to 0 when negative g values not significantly different from 0 (t-test between k\_dil and K\_N) were obtained. Thus, the average k\_N represented mu\_N and the average k\_NoN represented mu\_0 (Murrell et al., 2002; Chen et al. 2009). Negative g values, significantly different from 0 (i.e. higher growth in the WSW treatment than in the diluted), represent a violation of the method's assumption. In such cases, g was reported as undetermined, and k in the undiluted bottles represented mu\_N and mu\_0. Uncertainties relative to mu\_N and mu\_0 were estimated from the standard deviations of the k\_N and k\_NoN triplicate values.

# Data Processing

Procedures for retrieving CTD and incubation temperature and light data as well as for quality-controlling chlorophyll data are documented at: <https://github.com/pmarrec/nes-lter-chl-cleaning>. Raw data are included in this repo.

Calculation of the growth and grazing rates is documented here: <https://github.com/pmarrec/nes-lter-rate-calculation-chl>

### Raw fluorescence data

The raw fluorescence data for each cruise are stored in csv files in the "chl-grazing-experiment-raw" folder. The csv files contain the cast and Niskin bottle numbers (in text format, with '' to avoid considering some multiple cast/Niskin entries as dates), the measured Fo, Fa, blank, blank\_acid data with treatment information (T0\_TF, dilution, nutrient\_treatment, light\_level, replicate\_bottle and replicate\_chl). The files also include the vol\_filtered, the vol\_extracted, the calibration coefficient Fs and r and the start/end datetime of the incubations. Empty (NaN) columns for: date\_time\_utc\_sampling, latitude, longitude, depth, temperature\_sampling, nearest\_station, distance, incubation\_tank, temperature\_incubation\_avg, temperature\_incubation\_std, are there for retrieving these additional data from the CTD files in the REST API (<https://github.com/WHOIGit/nes-lter-ims/wiki/Using-REST-API-to-access-NES-LTER-data>) and from the csv files containing the temperature recorded in the incubation tanks during each cruise.

### Retrieving CTD data

The chl\_grazing\_experiment\_retrieve\_ctd\_data Matlab script is used to retrieve the date\_time\_utc\_sampling, latitude, longitude, depth, and temperature\_sampling directly and automatically from the CTD files stored in the REST API.

### Retrieving temperature during incubation

The Matlab script chl\_grazing\_experiment\_retrieve\_temp\_inc\_data.m is used to retrieve the temperature in the incubation tanks during dilution experiments. It acquires the mean and standard deviation of temperature recorded by the HOBO data loggers in the different incubators. Because of the lack of records in terms of which bottles were incubated in which specific tank (there are up to 3 CRUISE\_temp\_inc\_X.csv files for each cruise), the mean/std in each tank are retrieved and the values with the lowest temperature difference are kept and saved automatically.

### Chl-a calculation

The chl\_grazing\_experiment\_chl\_calc.m Matlab script is used to calculate the chl-a and phaeopigment concentrations, after calculation of Fo-blank, Fa-blank, and Fo/Fa ratios.

### Chl-a quality check

The chl\_grazing\_experiment\_fofa\_cleaning.m Matlab script is used to perform the 1st step of data quality check (aka cleaning). This first step is based on 2 criteria: 1. Fo/Fa within 1-3 range, 2. Fo/Fa witihn +/- 2 StdDev confidence interval for a given type of filter All the values that don't fit these criteria are flagged as questionable with a iode\_quality\_flag = 3. All the other values are flagged as good with a iode\_quality\_flag = 1

The chl\_grazing\_experiment\_chl\_conc\_clean.m Matlab script is used to perform the 2nd step of the cleaning based on the Chl-a concentrations. This second step is based on 2 criteria: 1. All negative Chl-a conc are flagged as questionable/suspect with iode\_quality\_flag = 3 2. For each station/depth/treatment/triplicate value: Each triplicate value should fall within 2 %CV of the mean value of the triplicate with a QC flag = 1. %CV is considered as the mean %CV obtained with a given type of filter (GFF/10µm) at T0 and at TF. All the values that don't fit these criteria are flagged as questionable with iode\_quality\_flag = 3. All the other values are flagged as good with iode\_quality\_flag = 1.

The chl\_grazing\_experiment\_chl\_conc\_clean\_special.m Matlab script is to correct T0 Chl-a concentration for few stations. In some cases (described below), the values of the T0 dilution were missing, making the rate calculation impossible. In these cases, the dilution values obtained from the other filters or from Flow Cytometry (FCM) were used: 
1. EN661 - L2: T0 >0&<200 Chl-a dilution values were way too high (>60%), while the dilution obtained from FCM and 10 µm filters gave the same dilution value of 23%. T0 diluted >0&<200 Chl-a concentration were then set as 23% of T0 WSW >0&<200 Chl-a concentration. 
2. EN668 - L6-D2: All T0 dilution values (>0&<200, >10&<200 and >0&<10) were questionable with dilution ranging from 43% to 76%, while according to the FCM we had 20% dilution. T0 WSW >0&<200 values look correct when compared to post-calibrated underway fluorescence. All the T0 WSW values are then considered good and are set as T0 dilution = 20% T0 WSW.

### Apparent growth rate "k" calculation

The chl\_grazing\_experiment\_k\_values.m Matlab script is used to compute the apparent growth rates k obtained during the dilution (grazing) experiments.

It creates a new table for each cruise gathering all the calculated k-values (apparent growth rates) for each treatment and filter type. The duration of each incubation is calculated from the date\_time\_utc\_end and the date\_time\_utc\_start for each experiment. Mean T0 chl-a concentration is calculated from replicates with iode\_quality\_flag = 1. T0 WSW mean Chla (Total = Chla, >10um = Chlau10, <10um = Chlad10) are reported in the new table, in addition to the % of Chl-a </>10um (Chlad10per and Chlau10per). Chlad10 = Chla - Chlau10. If Chlad10 < 0, Chlad10 = 0, Chlad10per = 0% and Chlau10per = 100%. k are calculated from each TF value. Up to 6 k values are then obtained for each treatment (dilution/nutrient/light) and filter type (>0&<200, >10&<200). Note that from cruise EN687 onward, up to 9 k values were obtained for 20WSW and WSW+N treatments because of the addition of another replicate bottle to achieve triplicate incubation bottles (a, b, and c).

Based on >0&200 (GFF) and >10&<200 (10um filters, u10 = up 10), >0&<10 (d10 = down 10) Chl-a values and then corresponding k values are calculated. For each triplicate, Chl-a d10 tripilcate values are calculated as the difference between the mean Chl-a value on >0&<200 and individual triplicate Chl-a values of >10&<200. Only data with QC = 1 are considered. If Chl-a d10 <0, then Chl-a conc and k are set to NaN.

### Phytoplankton growth and microzooplankton grazing calculation

The chl-grazing\_experiment\_rates.m Matlab script is used to compute phytoplankton growth rates (mu\_0), microzooplankton grazing rates (g; column 'grazing' in the product data table), apparent growth rates in nonamended nutrient treatment (WSW NoN, k\_NoN) and phytoplankton growth rates in nutrient-amended treatments (mu\_N = g + k\_N). Associated errors (std) were estimated for all these rates. Note that k\_NoN and mu\_N were estimated only when there was apparent nutrient limitation.

From this script, a new table for each cruise gathering all the calculated rates for each treatment and filter type from the k (apparent growth rates) values and the associated data and metadata is created.

The chl\_grazing\_experiment\_concatenate\_order\_rates.m Matlab script is used to concatenate the CRUISE rate table to get one final table with all the cruises together and reorganize the table by cruise, inverse latitude (station nb), and size fraction.

The chl\_grazing\_experiment\_rates\_QC.m Matlab file is used to Quality Check (QC) and rename some values of the rate data based on the following criteria: 
1. Values of grazing rate (g) and g_std below 0 are converted to NaN because they violate the assumptions of the dilution method.
2. If the difference between sampling temperature and temperature in incubator <-4 °C or > 4° C, iode\_quality\_flag = 3 (questionable). 
3. For light level = 100% (EN644), iode\_quality\_flag = 3 (questionable). It was too much light intensity for the experiment and the phytoplankton got "burned/fried". 
4. If dilution > 0.4 (40%), iode\_quality\_flag = 3 (questionable). The optimal dilution level for the 2-points method is <40% (Morison and Menden-Deuer, 2017).
5. If Chlad10 (>0&<10 µm) or Chlau10 (>10&<200 µm) concentrations are < 0.02 mg/m^3, the rates for these size fractions are considered questionable (iode\_quality\_flag = 3).
6. If Chlad10per (<10um) or Chlau10per (>10um) relative contribution to total Chl-a are < 0.02 (2%), the rates for these size fractions are considered questionable (iode\_quality\_flag = 3).

### Note about missing value codes

As documented in the data table column descriptions, the meaning of a missing value differs by column. For the chlorophyll columns, a missing value indicates that chlorophyll sample data are not available. For mu\_0 and mu\_0\_std, a missing value results when mu\_0 cannot be determined due to lack of chlorophyll data with IODE quality flag = 1 or because the experiment was performed only with nutrient addition (no control). For grazing and grazing\_std, a missing value indicates the parameter is not determined because g < 0, which is a violation of the dilution method's assumption. For mu\_N and mu\_N\_std, a missing value indicates the experiment was not nutrient-limited.

# Reuse of chlorophyll data

Chlorophyll data in this product are re-used from the NES chlorophyll transect rosette package (knb-lter-nes.8), which should be considered the authoritative source:

Sosik, H.M., T. Rynearson, S. Menden-Deuer, and OOI CGSN Data Team. 2021. Size-fractionated chlorophyll from water column bottle samples collected during NES-LTER Transect cruises, ongoing since 2017. ver 1. Environmental Data Initiative. <https://doi.org/10.6073/pasta/798bda0e9ddfeba20f2266e64cf4dd40> (Accessed 2023-05-11).

Columns Chla and Chlau10 in this growth and grazing product are equivalent to the average of chl replicates for size fractions >0&<200 and >10&<200 in the chlorophyll transect rosette package. Note that in this growth and grazing product, chlorophyll values are repeated for all rows of each station.

# Data package assembly

Package assembly was performed in R Markdown. Further documentation can be found on GitHub, at <https://github.com/WHOIGit/nes-lter-growth-grazing-chl>.

We assured that all geographic (latitude, longitude, depth, station) and temporal (date\_time\_utc\_sampling) values, as well as other metadata (cast, Niskin, temperature\_sampling) were as expected, and that chlorophyll values matched those contributed to the forthcoming version 2 of the chlorophyll transect rosette product mentioned above.

# Differences from previous version

In Version 2: 
- Data for 9 cruises were added. 
- Chlorophyll concentration data from the zero time point of the incubations were added. 
- Records at depths greater than surface were added (version 1 included only surface measurements).
- Some values were changed (e.g., EN608 cast 8 15% light-level) 
- The data table structure has been updated from wide to long format and includes 30 columns instead of the prior 41 columns. Salinity is not reported, and the version 1 columns denoting size fractions for growth and grazing parameters are instead denoted by the size_fraction column. 
- The following columns were renamed from the previous version:

| Version 1       | Version 2              |
|-----------------|------------------------|
| bottle          | niskin                 |
| date\_time\_UTC   | date\_time\_utc\_sampling |
| temp            | temperature\_sampling   |
| light\_treatment | light\_level            |
| mu\_N\_Std        | mu\_N\_std               |
| grazing\_N\_Std   | grazing\_N\_std          |

-   The following columns were added in version 2: incubation\_tank, temperature\_incubation\_avg, temperature\_incubation\_std, size\_fraction, Chla, Chlad10, Chlau10, Chlad10per, Chlau10per, duration\_incubation, dilution, iode\_quality\_flag

# References

Chen, B., Liu, H., Landry, M.R., DaI, M., Huang, B., Sune, J., 2009. Close coupling between phytoplankton growth and microzooplankton grazing in the western South China Sea. Limnology and Oceanography 54, 1084--1097. <https://doi.org/10.4319/lo.2009.54.4.1084>

Graff, J.R., Rynearson, T.A., 2011. Extraction method influences the recovery of phytoplankton pigments from natural assemblages: Chlorophyll extraction method artifacts. Limnology and Oceanography: Methods 9, 129--139. <https://doi.org/10.4319/lom.2011.9.129>

Jespersen AM, Christoffersen K., 1987. Measurements of Chlorophyll a from phytoplankton using ethanol as a solvent. Archiv Fur Hydrobiologie 109:445454.

Landry, M.R., Hassett, R.P., 1982. Estimating the grazing impact of marine micro-zooplankton. Marine Biology 67, 283--288. <https://doi.org/10.1007/BF00397668>

Landry, M.R., Haas, L.W., Fagerness, V.L., 1984. Dynamics of microbial plankton communities: experiments in Kaneohe Bay, Hawaii. Marine Ecology Progress Series 16, 127--133. <https://doi.org/10.3354/meps016127>

Landry, M.R., Brown, S.L., Rii, Y.M., Selph, K.E., Bidigare, R.R., Yang, E.J., Simmons, M.P., 2008. Depth-stratified phytoplankton dynamics in Cyclone Opal, a subtropical mesoscale eddy. Deep Sea Research Part II: Topical Studies in Oceanography 55, 1348--1359. <https://doi.org/10.1016/j.dsr2.2008.02.001>

Murrell, M.C., Stanley, R.S., Lores, E.M., DiDonato, G.T., Flemer, D.A., 2002. Linkage between microzooplankton grazing and phytoplankton growth in a Gulf of Mexico estuary. Estuaries 25, 19--29. <https://doi.org/10.1007/BF02696046>

Morison, F., Menden-Deuer, S., 2017. Doing more with less? Balancing sampling resolution and effort in measurements of protistan growth and grazing-rates: Measuring plankton growth and grazing. Limnology and Oceanography: Methods 15, 794--809. <https://doi.org/10.1002/lom3.10200>
