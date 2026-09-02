This readme file was generated on [YYYY-MM-DD] by Alexander Tekles

# GENERAL INFORMATION

Title of Data set: Data and code for "Same-gender citations do not indicate a substantial gender homophily bias"
Description: This repository contains the (pre-processed) data and code that was used for generating the results presented in the paper "Same-gender citations do not indicate a substantial gender homophily bias".

Author/Principal Investigator Information
Name: Tekles, Alexander
ORCID: n/a
Institution: n/a
Email: alexander.tekles@soziologie.uni-muenchen.de <Note: might be out of date since he is no longer listed among the staff members of the LMU Sociology department>

Date of data collection: n/a

Geographic location of data collection: n/a

Information about funding sources that supported the collection of the data: n/a

# SHARING/ACCESS Data

Licenses/restrictions placed on the data: CC BY-NC-SA 4.0 (https://creativecommons.org/licenses/by-nc-sa/4.0/) 

Links to publications that cite or use the data: https://doi.org/10.1371/journal.pone.0274810

Links to other publicly accessible locations of the data: n/a

Links/relationships to ancillary data sets: n/a

Was data derived from another source? If yes, list source(s): 

* Faculty Opinions Data (Link?) 
* Web of Science (Link?) 

# DATA & FILE OVERVIEW

**File List**: 

* focals.csv (data on the level of focal papers from the Faculty Opinions data)
* focals_sections.csv (keywords provided in the Faculty Opinions data for each focal paper)
* focal_pairs_fosims.csv (pairs of focal papers from the Faculty Opinions data) 
* focal_pairs_fosims_sc.csv (pairs of focal papers from the Faculty Opinions data; including self-citations)
* focal_pairs_citedrefsims.csv (pairs of focal papers from the Faculty Opinions data)
* focal_pairs_keywordsims.csv (pairs of focal papers from the Faculty Opinions data)  
* focal_pairs_subjsims.csv (pairs of focal papers from the Faculty Opinions data) 
* focal_pairs_fosims_cited.csv (pairs of focal papers from the Faculty Opinions data) 
* focal_pairs_fosims_cgender.csv (pairs of focal papers from the Faculty Opinions data; based on more restrictive gender assignments)
* focal_pairs_abstrsims.csv (pairs of focal papers from the Faculty Opinions data 
* wos_focal_pairs_abstrsims.csv (pairs of focal papers from WoS)
* analyses_focals.R (This script produces the figure showing the estimates of the regression analyses on the level of focal papers. The script uses the files `focals.csv` and `focals_sections.csv`.)
* analyses_pairs.R (This script produces figures showing the results of all analyses of paper pairs. In the first few lines, you can specify which results the script should produce. There are several vectors containing parameters representing the possible settings for which results can be produced. The script then iterates over all possible combinations of parameters. For example, in the vector `fo_data_opts`, the value `T` specifies to produce the results based on the Faculty Opinions data and the value `F` specifies to compute the results based on the WoS data. Changing the corresponding line from `fo_data_opts <- c(T, F)` to `fo_data_opts <- c(T)`
would mean to only compute the results based on the Faculty Opinions data (instead of both the Faculty Opinions and the WoS data). This particular adjustment may be helpful because it saves a lot of runtime (the file containing the WoS data is much larger than the other files).)
* studies_results.R (This script produces the figure showing the overview of results of previous studies on gender homophily in citations.)

**Relationship between files, if important:** 

The file gender_homophily_data_fo.tar.gz is a tarball that contains all data (CSV) files for the Faculty Opinions data. The file gender_homophily_data_wos.tar.gz contains all data (CSV) files for the Web of Science (WoS) data. The tarballs have to be unpacked to access the CSV files. This can be done via command line with the following commands: 

`tar -xzf <path_to_folder>gender_homophily_data_fo.tar.gz -C <path_to_target_folder>`

`tar -xzf <path_to_folder>gender_homophily_data_wos.tar.gz -C <path_to_target_folder>`

Make sure to replace `<path_to_folder>` with the path to the folder containing the tarballs and `<path_to_target_folder>` with the path to the folder where you want the CSV files to be unpacked.

All R scripts contain a function call of `setwd()` in the first few lines. The argument of this function should be the path to the folder containing the CSV files. This folder should also contain a folder named `res`, where the results of the analyses are saved.

Additional related data collected that was not included in the current data package: n/a

# METHODOLOGICAL INFORMATION <Excluded for brevity reasons>

Description of methods used for collection/generation of data:

Methods for processing the data:

Instrument- or software-specific information needed to interpret the data: <include full name and version of software, and any necessary packages or libraries needed to run scripts>

Standards and calibration information, if appropriate:

Environmental/experimental conditions:

Describe any quality-assurance procedures performed on the data:

People involved with sample collection, processing, analysis and/or submission: