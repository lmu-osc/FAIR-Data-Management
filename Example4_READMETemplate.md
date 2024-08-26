This readme file was generated on [YYYY-MM-DD] by Dominik Deffner


# GENERAL INFORMATION

**Title of Data set**: Collective incentives reduce over-exploitation of social information in unconstrained human groups
Description: This repository contains the full data and scripts to reproduce all analyses and figures as well as the experimental game itself used in Deffner, D., Mezey, D., Kahl, B., Schakowski, A., Romanczuk, P., Wu, C. & Kurvers, R. (accepted, in principle, at Nature Communications): “Collective incentives reduce over-exploitation of social information in unconstrained human groups”


Author/Principal Investigator Information
Name: Deffner, Dominik
ORCID:
Institution:
Email:
Date of data collection: 2022-07-05 to 2022-09-21

Geographic location of data collection: Max Planck Institute for Human Development

Information about funding sources that supported the collection of the data: n/a

# SHARING/ACCESS Data

Licenses/restrictions placed on the data: CC BY 4.0 / Apache License 2.0 

**Links to publications that cite or use the data**: https://psyarxiv.com/p3bj7/ 

Links to other publicly accessible locations of the data: https://github.com/DominikDeffner/VirtualCollectiveForaging/tree/0.1.0?tab=readme-ov-file

Links/relationships to ancillary data sets: n/a

Was data derived from another source? If yes, list source(s): n/a

# DATA & FILE OVERVIEW

**File List**: 

"master_file.r" sources all other scripts and implements the entire project workflow from raw Unity data to plots in the manuscript.

The "Scripts" folder contains all relevant R scripts for data processing and analysis:

- "functions.R" loads all required functions and packages
- "data_prep.R" runs data preparation script to construct dataframes for analysis from raw Unity outputs
- "HiddenMarkovModels_prep.R" contructs extended dataframe and stan data list for Social Hidden Markov Decision model
- "Behavior_prep.R" computes behavioral summary statistics for each player/group and round
- "Behavior_individual_level.R" runs and plots behavioral analyses at individual level
- "Behavior_group_level.R" runs and plots behavioral analyses at group level
- "Behavior_main_plot" produces main behavioral plot (Fig.2)
- "Behavior_solitary.R" runs and plots behavioral analyses for solo control condition
- "HiddenMarkovModels_baseline.R" runs baseline Social Hidden Markov Decision model and produces main text plots
- "Viterbi.r" computes most likely state sequences for all participants through Viterbi algorithm
- "HiddenMarkovModels_ESM_Plots.R" produces supplementary HMM plots
- "HiddenMarkovModels_temporal.R" runs and plots temporal Social Hidden Markov Decision model
- "CollectiveDynamics.R" runs and plots collective visual-spatial dynamics analyses using time-lagged Gaussian-process regressions

The "Stan model code" folder contains stan files for the (baseline and time-varying) Social Hidden Markov Decision model as well as the time-lagged Gaussian-process model
- "m_SHMDM.stan" is the baseline HMM (called in "HiddenMarkovModels_baseline.R")
- "m_SHMDM_temporal.stan" is the time-varying HMM (called in "HiddenMarkovModels_temporal.R")
- "m_temporal_success.stan" is monotonic-effect model for success over time (called in "HiddenMarkovModels_temporal.R")
- "m_time_laggedGP.stan" is the time-lagged Gaussian-process model to analyze collective visual-spatial dynamics (called in "CollectiveDynamics.R")

The "Data" folder contains all raw data for both "Group" and "Solo" conditions. Each sub-folder contains data from one experimental session. There are separate .txt files for participant demographics and for player and patch data from each round (indexing starts at 0). Variable names should be quite descriptive, but please get in touch in case anything is unclear.

**Relationship between files, if important**: included above

Additional related data collected that was not included in the current data package: n/a

# METHODOLOGICAL INFORMATION

Description of methods used for collection/generation of data:

Methods for processing the data:

Instrument- or software-specific information needed to interpret the data: <include full name and version of software, and any necessary packages or libraries needed to run scripts>

Standards and calibration information, if appropriate:

Environmental/experimental conditions:

Describe any quality-assurance procedures performed on the data:

People involved with sample collection, processing, analysis and/or submission:
