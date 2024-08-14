This readme file was generated on **November 3, 2021** by **Sarah Polk and Maike Kleemeyer**

# GENERAL INFORMATION

**Title of Data set:** ICED MPMs
**Description: Investigating reliability of estimates of multiparameter mapping**


Author/Principal Investigator Information
**Name:** Maike Kleemeyer
ORCID: 0000-0002-9388-5535
Institution: n/a
Email: n/a
Date of data collection: n/a

Geographic location of data collection: n/a

Information about funding sources that supported the collection of the data: n/a

# SHARING/ACCESS Data

Licenses/restrictions placed on the data: No License

Links to publications that cite or use the data: https://doi.org/10.1101/2021.11.10.467254

Links to other publicly accessible locations of the data: https://git.mpib-berlin.mpg.de/plasticity/aktiv/hmri_longitudinal/tree/main

Links/relationships to ancillary data sets: n/a

Was data derived from another source? If yes, list source(s): n/a

# DATA & FILE OVERVIEW

File List: 
- Gitlab
The linked gitlab repository contains all scripts for processing the imaging data including descriptions of their purpose as well as the required folder structure to rerun the scripts.
- Data
The data folder contains the extracted data from the 11 different regions of interest (gray matter, white matter, pars triangularis of the inferior frontal gyrus, pars opercularis of the inferior frontal gyrus, orbitofrontal cortex, anterior cingulate cortex, precuneus, poster middle temporal gyrus, caudate, putamen, and pallidum) for each parameter map (MTsat, PD, R1, R2*) for each day (one and two) and each session (1 and 2). Regions of interest were taken from the Harvard-Oxford atlas as included in FSL 5.0.
- extract_from_ROIs
This folder contains the script used to extract means and standard deviations from the predefined regions of interest.
- Scripts
The scripts folder contains the models and ought to be run on the derived data in the data folder given the following structure:
/data
/data/MPMsExtractedWide.csv
/data/MPMsExtractedWideStd.csv
/scripts
/scripts/CalcICCsWithCIs.R
/scripts/ICED_MPMs_analysis.R

Relationship between files, if important: n/a

Additional related data collected that was not included in the current data package: n/a

# METHODOLOGICAL INFORMATION <excluded for brevity reasons>

Description of methods used for collection/generation of data:

Methods for processing the data:

Instrument- or software-specific information needed to interpret the data: <include full name and version of software, and any necessary packages or libraries needed to run scripts>

Standards and calibration information, if appropriate:

Environmental/experimental conditions:

Describe any quality-assurance procedures performed on the data:

People involved with sample collection, processing, analysis and/or submission: