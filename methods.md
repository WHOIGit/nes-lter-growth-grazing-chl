# Sample Collection

At each station, hydrographic data of depth, temperature, and salinity
were collected with a SBE911 (Seabird Electronics Inc.) CTD-rosette
system. Seawater for the experiments was collected near the surface
(1.6-7 m) using multiple Niskin bottles and sometimes from different CTD
casts at a given location. Cast and bottle numbers are reported in the
data table. Depth, temperature and salinity values of the seawater
collected for the experiments reported in the data table are averaged
from bottle summary files produced with Seabird software onboard ship
and have not been corrected to salts.

# Experimental Set-Up

Rates of phytoplankton growth and microzooplankton grazing were
quantified using a 2-point modification of the dilution method (Morison
and Menden-Deuer, 2017). Whole seawater (WSW) was gently transferred
from a Niskin to a 10 L polycarbonate carboy through a 200 µm mesh to
remove mesozooplankton predators (e.g. copepods). Diluent was prepared
by gravity filtration through a 0.2 µm membrane filter capsule (PALL)
from the Niskin to the carboys. The appropriate amount of WSW was added
to the filtered water to obtain a 20 percent WSW dilution (20WSW). The
carboys were covered by black trash bags and gently mixed while water
was siphoned into duplicate 1.2 L clear polycarbonate bottles. To ensure
the gross growth rate of the phytoplankton was not dependent upon
dilution, a central assumption of the dilution method (Landry and
Hasset, 1982), incubation bottles were amended with macronutrients (10
µM SiO4, 10 µM NO3, 1 µM PO4). An additional set of WSW bottles without
additional nutrients was added to assess nutrient limitation or toxicity
effects. For each dilution (20WSW and WSW), nutrient (nutrient amended
and without nutrient) and light (high and low light, see below)
treatment, incubation bottles were duplicated.

Bottles were incubated for 24 h in a clear deck-board, flow through, 1
m\^3, incubator. Surface water was incubated at two light-levels that
simulated the contrasting light conditions (e.g. sunny/cloudy weather,
well-mixed/stratified water column) under which phytoplankton could be
growing in the surface ocean. Mesh, screen, bags were used to create
High Light (HL) and Low Light (LL) treatments that simulated 65 percent
and 15 percent of light attenuation. The incubator was free of overhead
obstructions to avoid shading during the day and covered by a tarp at
night to minimize light pollution from deck lighting. Natural movement
of the ship kept the bottles in the incubator agitated over the
incubation period. Temperature within the incubators was maintained
equivalent to current surface temperature through continuous
flow-through from the ship seawater system. Temperature and light in the
incubators were monitored at 5-minute intervals with a Hobo (Onset) data
logger. Temperature and light measurements recorded during each of the
incubation experiments are available in .csv files following the links
present in the last column of the data table.

# Phytoplankton Growth and Protist Grazing Rate Estimates

Initial (T0) chlorophyll-a (Chl-a) concentration was determined from
triplicate 120-150 mL subsamples from carboys used to fill incubation
bottles. Final Chl-a concentration (TF) was determined from triplicate
120-150 mL subsamples from bottles at the end of the incubation. The
extraction method followed Graff and Rynearson (2011) except here we
used 95 percent ethanol as a solvent (Jespersen and Christoffersen,
1987). Extracted Chl-a concentration was determined using a Turner AU10
fluorometer after a 12 h extraction period. In addition, the size
structure of the initial phytoplankton community was characterized from
T0 triplicate size-fractionated Chl-a samples (greater than 0.7 µm GF/F,
greater than 5 µm, greater than 10 µm, and greater than 20 µm). At TF,
size-fractionated Chl-a concentration at 10 µm were also measured for
20WSW and WSW nutrient amended bottles. During the first winter cruise
in 2018 (EN608) size fractionation was only performed on bottles
incubated under high light conditions.

Phytoplankton growth rates and protist grazing rates were estimated from
24 h changes in Chl-a concentration. For each incubation bottle, the
apparent growth rates (k, d\^-1) were calculated as: k=1⁄t×ln(C_t⁄C_0)

where t is the incubation time (d) and C_t and C_0 the final and initial
Chl-a concentration (µg L\^-1), respectively.

Protist grazing rates (g, d\^-1) were estimated with the equation:

g=((k_d-k_N))⁄((1-x))

where k_d and k_N are the apparent growth rates in 20WSW and WSW
nutrient amended treatments, respectively, and x is the achieved
fraction of WSW in the diluted treatment calculated from T0 Chl-a in
20WSW and WSW (Landry et al., 1984). Accordingly, the instantaneous, or
in situ, growth rate (mu_0, d\^-1) was estimated as in (Landry et al.,
2008):

mu_0=g+k_NoN

where k_NoN is apparent phytoplankton growth rate k without nutrient
addition.

The potential for nutrient limitation was assessed by comparing apparent
phytoplankton growth rates k in nutrient amended (k_N) and nonamended
(k_NoN) replicates using a paired t-test. If a significant difference
was found (p below 0.05) between k_N and k_NoN, nutrient-amended growth
rates (mu_N, d\^-1) were also calculated as mu_N = g + k_N. Otherwise,
all k_N and k_NoN triplicate of replicate values were used to calculate
both g and mu_0.

Since size fractionation at 10 µm was performed only on nutrient amended
samples, growth rates reported on greater than 10 µm and less than 10 µm
fractions in this study were nutrient-amended growth rates (mu_N) when
nutrient limitation was observed. If no nutrient limitation was
observed, mu_N obtained is equivalent to mu_0.

The uncertainty of g estimates was quantified using the standard error
of the slope fit from a linear regression between replicate k values and
dilution levels. When the slope obtained was not significantly different
from zero (p higher than 0.05), g was set to 0. Thus, the average k_N
represented mu_N and the average k_NoN represented mu_0 (Murrell et al.,
2002; Chen et al. 2009). A significant positive slope (i.e. higher
growth in the WSW treatment than in the diluted) represents a violation
of the method's assumption. In such cases, g was reported as
undetermined, and k in the undiluted bottles represented mu_N and mu_0.
Uncertainties relative to mu_N and mu_0 were estimated from the standard
deviations observed on k_N and k_NoN triplicate values.

# Data Cleaning

Data cleaning (i.e., separating numerical and categorical variables,
referring to multiple casts and bottles, and assuring date and time of
sampling) and metadata template assembly were performed in R Markdown.
Further documentation can be found on GitHub, at
https://github.com/WHOIGit/nes-lter-growth-grazing-chl.

# Quality Assurance

We assured that all values reported in the clean data table for
geographic (latitude, longitude, depth, station), temporal
(date_time_UTC, date_time_start_UTC, date_time_end_UTC), and other
cruise metadata and data (cast, bottle, temp, sal) were aligned with
other NES-LTER data products.

# References

Chen, B., Liu, H., Landry, M.R., DaI, M., Huang, B., Sune, J., 2009.
Close coupling between phytoplankton growth and microzooplankton grazing
in the western South China Sea. Limnology and Oceanography 54,
1084--1097. https://doi.org/10.4319/lo.2009.54.4.1084

Graff, J.R., Rynearson, T.A., 2011. Extraction method influences the
recovery of phytoplankton pigments from natural assemblages: Chlorophyll
extraction method artifacts. Limnology and Oceanography: Methods 9,
129--139. https://doi.org/10.4319/lom.2011.9.129

Jespersen AM, Christoffersen K. 1987. Measurements of Chlorophyll a from
phytoplankton using ethanol as a solvent. Archiv Fur Hydrobiologie
109:445454.

Landry, M.R., Hassett, R.P., 1982. Estimating the grazing impact of
marine micro-zooplankton. Marine Biology 67, 283--288.
https://doi.org/10.1007/BF00397668

Landry, M., Haas, L., Fagerness, V., 1984. Dynamics of microbial
plankton communities: experiments in Kaneohe Bay, Hawaii. Marine Ecology
Progress Series 16, 127--133. https://doi.org/10.3354/meps016127

Landry, M.R., Brown, S.L., Rii, Y.M., Selph, K.E., Bidigare, R.R., Yang,
E.J., Simmons, M.P., 2008. Depth-stratified phytoplankton dynamics in
Cyclone Opal, a subtropical mesoscale eddy. Deep Sea Research Part II:
Topical Studies in Oceanography 55, 1348--1359.
https://doi.org/10.1016/j.dsr2.2008.02.001

Murrell, M.C., Stanley, R.S., Lores, E.M., DiDonato, G.T., Flemer, D.A.,
2002. Linkage between microzooplankton grazing and phytoplankton growth
in a Gulf of Mexico estuary. Estuaries 25, 19--29.
https://doi.org/10.1007/BF02696046

Morison, F., Menden-Deuer, S., 2017. Doing more with less? Balancing
sampling resolution and effort in measurements of protistan growth and
grazing-rates: Measuring plankton growth and grazing. Limnology and
Oceanography: Methods 15, 794--809. https://doi.org/10.1002/lom3.10200