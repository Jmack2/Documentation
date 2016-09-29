##ET_Redux Documentation Overview

ET_Redux is a stand alone desktop application, which ET_Redux was produced by CIRDLES as the successor to U-Pb_Redux on January 22, 2015. The purpose of ET_Redux is to integrate automatic data archiving and results into the NSF-sponsored Geochron community database. ET_Redux produces analysis results as an 'aliquot' XML file, which can be exported to Geochron or stored and shared as desired.

##Information for use of Documentation
The documentation below is essentially a set of step by step instructions on how to operate the software. For auditory and visual learners, youtube video tutorials will be included among the written instructions, so there will be a video demonstration of ET_Redux operations from a computer desktop.

##Concept of operations
The objective of ET_Redux is to extend its architecture to U-series analyses in addition to IDTIMS and LA-ICPMS U-Pb data reduction, uncertainty propagation, and visualization for any U-bearing phase. ET_Redux supplies sophisticated graphical and statistical tools for data analysis and compilation. These include interactive data tables, concordia and weighted mean plots, dynamic decomposition of uncertainties into contributions from individual sources, and algorithms for propagation of systematic uncertainties in tracer calibration and decay constants. ET_Redux also generates these outputs as publication-ready vector graphics files.

##Policies that affect the system
ET_Redux is sponsored by EARTHTIME and the Nationl Science Foundation.

###Project

##Starting ET_Redux and starting data reduction

Open ET_Redux and when the window opens click “Project” in the upper left-hand corner. Then, click New Project from Raw Data and select LA-ICP-MS. Selecting this option brings up the Project Manager window. Once the window is open fill in the designated data fields:
	
	•	Project name
	•	Handling Protocol: Laserchron Element II Folder of .dat files
	•	Raw data template: Laserchron Element II 202-235-238
	•	Analysis purpose: Detrital Spectrum
	
Then, press “Prepare to Load/Process Raw Data.” Select your data folder and click Open, while making sure that all files are in the same folder (especially .dat files and scanlist).
 Make sure that full uncertainty is checked and fill out the 

Primary Reference Material: FC1-Anorthosite from Forest Center

Now, you can begin the data reduction process. There are two different types of data reduction: live data reduction and the raw data manager.

####Sample
A single collection of a geologic material (usually rock or mineral) from one location. A sample has a lab specific name and a unique identifier such as the IGSN provided by SESAR.

Click Sample and then select ID-TIMS. The ID-TIMS Workflow Manager window will open. 

Fill in the designated fields:
	Local Sample Name
	Sample ID
	Aliquot Name
	Registry
	Analysis Purpose
	Set Physical Constants Model
