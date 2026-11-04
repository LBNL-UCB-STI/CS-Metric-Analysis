**Project Title:</b>National utility-based framework for evaluating U.S. work trip accessibility**

**Authors:** C. Anna Spurlock, Jessica Lazarus, Xiaodan Xu, Zachary A. Needell, Ling Jin, Mahyar Amirgholy, Joseph Y.J. Chow, Mona Asudegi

**Contact:** Mona Asudegi (mona.asudegi@dot.gov ); C. Anna Spurlock (caspurlock@lbl.gov)
************************************************
**Description:**
This repository contains the data and code necessary to reproduce the primary analysis and figures for the manuscript “National utility-based framework for evaluating U.S. work trip accessibility”. The analysis demonstrates a newly defined work travel accessibility metric characterizing the quality, as a monetized consumer surplus (CS), of travel for the purpose of work for every census tract in the continental United States. The analysis additionally demonstrates the correlation of that CS metric with median household income.

The code and data necessary for generation of the CS metric itself relies on data that is restricted and cannot be made public due to the terms of the data access agreement governing the access to those data for the researchers. Specifically, the National Household Travel Data (NHTS) data from 2017 with the census tract, in 2010 census geographies, of home location, and the origin and destination of all trips, were provided under this data access agreement. These data are necessary for estimation of the mode choice and destination choice models underpinning the CS metric. The data and code provided in this repository uses the generated census tract level cs metric output from the pipeline dependent on the proprietary data, and includes the code used to generate the figures, ANOVA analysis, and regression results presented in the second part of the main results section of the manuscript.
************************************************
**Repository Content:**
- \code - contains the Stata .do file that conducts the analysis.
- \raw - contains the initial dataset
- \process - contains interim data generated over the course of the analysis
- \figures - contains the results figures generated from running the analysis code
- \tables - contains the regression results and log output generated from running the analysis code
************************************************
**System Requirements & Dependencies**
- Programming Language: Stata/MP 18.0
- Key libraries/packages: the requirements.do file saved in the code/ directory can be run to install the two user-developed packages used in the primary code file for the analysis.
************************************************
**Installation**
- Clone the repository to a local computer with Stata installed
- Navigate to the local directory
- Ensure the repository's directory structure (/code, /raw, etc.) is maintained, as the analysis script relies on these relative paths. Instructions to this effect are provided in the 'code/CS analysis code.do' as well
- Open the 'code/CS analysis code.do' file in Stata and enter the local directory path in the two lines of the code where instructed
```
cd "<input path to local directory here>"
global dir "<input path to local directory here>"
```
************************************************
**Instructions for Reproduction:**
- Execute the 'code/requirements.do' file in Stata
- Execute the 'code/CS analysis code.do' file in Stata
************************************************
**Expected Output:** 
The \figures and \tables directories in this repository contain the two figures and three tables (in both .txt and .xml format) as well as a log file that will be generated in these directories locally when the code is executed as instructed. These output files can be separately downloaded from GitHub or saved in separate directories to directly compare to the output you generate when you execute the analysis to ensure your results reproduce these results.
************************************************
**Data Description & Availability:**
The code and data necessary for generation of the CS metric itself relies on data that is restricted and cannot be made public due to the terms of the data access agreement governing the access to those data for the researchers. Specifically, the National Household Travel Data (NHTS) data from 2017 with the census tract, in 2010 census geographies, of home location, and the origin and destination of all trips, were provided under this data access agreement. These data are necessary for estimation of the mode choice and destination choice models underpinning the CS metric. The data and code provided in this repository uses the generated census tract level CS metric output from the pipeline dependent on the proprietary data, and includes the code used to generate the figures and regression results presented in the second part of the main results section of the manuscript.
************************************************
**Data Dictionary:** 
A data_dictionary.xls inside the raw/ folder is made available. It includes a description of each column in the initial dataset in the raw/ folder.
************************************************
**How to Cite:**
If you use the data or code from this repository in your research, please cite the following manuscript:
Spurlock, C. Anna, Jessica Lazarus, Xiaodan Xu, Zachary A. Needell, Ling Jin, Mahyar Amirgholy, Joseph Y.J. Chow, Mona Asudegi (2027). "National utility-based framework for evaluating U.S. work trip accessibility". _Travel Behaviour and Society_, 4, 101425. https://doi.org/10.1016/j.tbs.2026.101425. 
************************************************
**Other Essential Information and Files:**
  
*Copyright Notice*

CQM-Analysis Copyright (c) 2025, The Regents of the University of California,
through Lawrence Berkeley National Laboratory (subject to receipt of any
required approvals from the U.S. Dept. of Energy). All rights reserved.

If you have questions about your rights to use or distribute this software,
please contact Berkeley Lab's Intellectual Property Office at
IPO@lbl.gov.

NOTICE.  This Software was developed under funding from the U.S. Department
of Energy and the U.S. Government consequently retains certain rights.  As
such, the U.S. Government has been granted for itself and others acting on
its behalf a paid-up, nonexclusive, irrevocable, worldwide license in the
Software to reproduce, distribute copies to the public, prepare derivative 
works, and perform publicly and display publicly, and to permit others to do so.

*License Agreement*
- See the full [LICENSE](LICENSE.md) file.

*Citation*

- CITATION.cff: [TO BE ADDED ONCE CITATION IS AVAILABLE - FOR NOW PLEASE DO NOT CITE]

