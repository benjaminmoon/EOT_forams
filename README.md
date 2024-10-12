# Data and code from 'Morphological trends in reticulate _Nummulites_ cross the Eocene-Oligocene transition'

[![DOI](https://zenodo.org/badge/850322011.svg)](https://zenodo.org/doi/10.5281/zenodo.13623171)

This code forms part of the supplementary material to:

KIRAN KOORAPATI, R., MOON, B. C. and COTTON, L. 2024. Morphological trends in reticulate _Nummulites_ across the Eocene-Oligocene transition. _Palaeontology_

This data is available from Zenodo at DOI: [doi/10.5281/zenodo.13623171](https://zenodo.org/doi/10.5281/zenodo.13623171) and should be cited as:


KIRAN KOORAPATI, R., MOON, B. C. and COTTON, L. 2024. Data from 'Morphological trends in reticulate _Nummulites_ across the Eocene-Oligocene transition'. Zenodo, doi: 10.5281/zenodo.13623171


Follow the code in `EOT_foram_analyses.Rmd`.

## Scripts

### EOT_foram_analyses.Rmd

The main analysis script. We used R version 4.2.1 and renv to manage the package versions. This should automatically install the relevant packages when used. These are stored in the .Rprofile and renv.lock files, and the renv folder, so keep these together.

The contents of the script include the following:

* Plotting variation in the data sets using box plots.
* Plot trends through time.
* Linear modelling of the evolutionary trends.
* Morphospace occupation of the EOT forams.

This script is documented internally. Follow the instructions there.

## Data files

All samples are from the Pande Formation of Tanzania and were collected during the Tanzania Drilling Project (TDP) cores 11, 12 and 17 (Nicholas _et al._ 2006; Pearson _et al._ 2008). Collection of the larger foraminifera was described by Cotton and Pearson (2011). The depth-age conversion of Pearson _et al._ (2008) ('old age model') was updated with Gradstein (2020) ('new age model'). Samples are archived with Dr Laura Cotton at the University of Copenhagen.

### Data2D.csv

A data table of measurements of _Nummulites_ taken in two-dimensions thin section. Includes the following columns:

* Sample.no: the sample number.
* depth: depth in the Tanzania Drilling Programme core (metres).
* Photos.available
* Notes
* Remarks
* Age..in.Ma.: age of the beds (using an old age model) (Ma). 
* Age_New: age of the specimen using the new age model (Ma).
* Planktonic_d13C, Planktonic_d18O: planktonic isotope ratios (‰). 
* Benthic_d13C, Benthic_d18O: bethic isotope ratios (‰).
* P1, P2, P3: proloculus size of the chambers (µm).
* D1, D2: deuteroconch size of the chambers (µm).
* R1, R2, R3, R4, R5, R6: radius of each whorl (µm).
* Radius: total radius (µm).
* TD: deuteroconch wall thickness (µm).
* T1, T2, T3, T4, T5: wall thickness of each whorl (µm).
* N1, N2, N3, N4, N5, N6, N: number of chambers in each whorl.
* WT: total number of whorls.
* Last.Complete.Whorl: number of the last complete whorl.
* No..of.chambers.in.final.whorl: number of chambers in the last whorl.
* Series: series, one of Eocene, EOT or Oligocene.
* CA1_Avg, CA2_Avg, CA3_Avg, CA4_Avg, CA5_Avg: average area of calcite by whorl (µm²).
* CL1_Avg, CL2_Avg, CL3_Avg, CL4_Avg, CL5_Avg: 
* CW1_Avg, CW2_Avg, CW3_Avg, CW4_Avg, CW5_Avg:
* CR1, CR2, CR3, CR4, CR5, CR: chamber ratios for each whorl, and total.
* CR_Avg: average total chamber ratio.
* PD

### Data3D.csv

A data table of measurements of _Nummulites_ taken in three-dimensions from CT scans. Includes the following columns:

* Sample Number.
* Remarks.
* Depth: depth in the TDP section (metres).
* Age: age of each bed (Ma).
* Planktonic_d13C, Planktonic_d18O: planktonic isotope ratios (‰).
* Benthic_d13C, Benthic_d18O: planktonic isotope ratios (‰).
* WT3D: total number of whorls.
* Calcite: total test volume (µm³).
* VP: volume of the proloculus (µm³).
* VD: volume of the deuteroconch (µm³).
* V1W, V2W, V3W, V4W, V5W, V6W: volumes of each whorl (µm³).
* C1W, C2W, C3W, C4W, C5W, C6W: number of chambers in each whorl.
* NV1W, NV2W, NV3W, NV4W, NV5W, NV6W: average chamber volume for each whorl (µm³).
* Diameter, Thickness: test shape (µm).
* DT: diameter/thickness ratio.
* CD: chamber volume of the deuteroconch (µm³).
* Series: series, one of Eocene, EOT or Oligocene.


### Isotopes_Modified.csv

A data table of isotope measurements through the Tanzania section with associated ages. Includes the following columns:

* sample: sample number.
* TDP12 Depth (m): depth recorded in the section (metres).
* TDP12 mcd (+58m): standardised depth.
* Age_new: age of each bed (Ma).
* d13C, d18O: planktonic isotope ratios (‰).
* d13C Cib, d18O Cib: benthic isotope ratios (‰).
* Remarks

## References

COTTON, L. J. and PEARSON, P. J. 2011. Extinction of larger benthic foraminifera at the Eocene/Oligocene boundary. _Palaeoceanography, Palaeoclimatology, Palaeoecology_, **311**, 281–296.

GRADSTEIN, F. M., OGG, J. G., SCHMITZ, M. D. and OGG, G. M. 2020. _Geologic Time Scale 2020_. Elsevier, 1357 pp.

NICHOLAS, C. J., PEARSON, P. N., BOWN, P. R., JONES, T. D., HUBER, B. T., KAREGA, A., LEES, J. A., McMILLAN, I. K., O'HALLORAN, A., SINGANO, J. M. and WADE, B. S. 2006. Stratigraphy and sedimentology of the Upper Cretaceous to Palaeogene Kilwa Group, southern coastal Tanzania. _Journal of African Earth Sciences_, **45**, 431–466.

PEARSON, P. N., McMILLAN, I. K., WADE, B. S., JONES, T. D., COXALL, H. K., BOWN, P. R. and LEAR, C. H. 2008. Extinction and environmental change across the Eocene-Oligocene boundary in Tanzania. _Geology_, **36**, 179–182.
