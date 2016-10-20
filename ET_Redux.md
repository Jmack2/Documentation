##ET_Redux Documentation Overview

ET_Redux is a stand alone desktop application, which ET_Redux was produced by CIRDLES as the successor to U-Pb_Redux on January 22, 2015. The purpose of ET_Redux is to integrate automatic data archiving and results into the NSF-sponsored Geochron community database. ET_Redux produces analysis results as an 'aliquot' XML file, which can be exported to Geochron or stored and shared as desired.

##Information for use of Documentation
The documentation below is essentially a set of step by step instructions on how to operate the software. For auditory and visual learners, youtube video tutorials will be included among the written instructions, so there will be a video demonstration of ET_Redux operations from a computer desktop.

##Concept of operations
The objective of ET_Redux is to extend its architecture to U-series analyses in addition to IDTIMS and LA-ICPMS U-Pb data reduction, uncertainty propagation, and visualization for any U-bearing phase. ET_Redux supplies sophisticated graphical and statistical tools for data analysis and compilation. These include interactive data tables, concordia and weighted mean plots, dynamic decomposition of uncertainties into contributions from individual sources, and algorithms for propagation of systematic uncertainties in tracer calibration and decay constants. ET_Redux also generates these outputs as publication-ready vector graphics files.

##Policies that affect the system
ET_Redux is sponsored by EARTHTIME and the National Science Foundation.

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

Click Sample and then select ID-TIMS. The ID-TIMS Workflow Manager window will open. 

Fill in the designated fields:
	Local Sample Name
	Sample ID
	Aliquot Name
	Registry
	Analysis Purpose
	Set Physical Constants Model

##Procedures
(-Youtube videos)

#####New Project from Raw Data
   	1.Open ET_Redux.
	2.Once you have opened ET_Redux, you will have three icons appear on your desktop, which is expected so don’t delete them.
	3.To start, click Project in the top left corner.
	4.Then, click New Project from Raw Data.
	5.Click, LA-ICP-MS
	6.Now, you will see the Project Manager interface; you have the ability to customize your project. You can start by entering your Project Name
		-Handling Protocol:
		-Raw data template:
		-Analysis purpose:
	10. Finally, press "Prepare to load/Process Raw Data." Then, you will be able to select your data folder and hit Open. Make sure that all necessary files are in the same folder!! .dat files and scanlist!
	12. Full Uncertainty should be checked!
	13. Primary Reference Material: FC1-Anorthosite from Forest Center
	14. Now we are ready to start the reduction process. From this point, you will be able to start live data reduction, which is explained below in the Raw Data Manager part of the documentation.

#####Live Data Reduction Processing (to be revised):
	1. Press, Save and Monitor/Process Raw Data
	2. Once launched you will have to wait for at least 3-4 analysis to be reduced before seeing any
data.
	3. To remove unwanted analysis, right click on the selected grain in your report table located below concordia, it will now be sent to the rejected fractions tab but will still be reduced
	4. To look at individual groups of grains (Standards or Unknowns), click on the sample name in the left hand column, a drop down menu will appear with all available groups to view on Concordia and on the PDF.
	5. To set different filters, adjust them under the PDF. To apply them to the Concordia plot, select apply filters under the Concordia.
	6. To change what ages are shown on the PDF, select one of the three ages (6/8, 6/7, or best age). We suggest the best age option.
	7. Best age filter can be changed while you are looking at unknowns in Concordia space
	8. When a grain is removed be patient, it will take until the next FC grain to update the session.
	9. If you need to refresh, hit Refresh Views
	10. Wait until the run has completed and proceed to Project Raw Data Manager section.

#####Project Raw Data Manager (to be revised)
	1. To make your view easier:
		a. Y-axis Scaling set to Independent
		b. Also press Show All Local Y-axis
	2. Proceed to look through all your reference materials to make sure your ratios are within the acceptable rages. It will be very clear when an analysis is bad. You will either see a very large scatter in data points or the fit line will be far off the data points.
	3. Once you have looked over your data points proceed to click on the Show Session button
	4. You will now be directed to the Fractionation Plots. Here is where we will remove any poorly behaved reference material analysis and hopefully achieve an MSWD of 1.0
	5. To remove a data point, hover over an errant black spot and right click. You will be asked to “exclude this fraction, click on it and the black dot will change to red indicating it has been removed.
	6. Once you have removed all unwanted data points you MUST hit refit, so that the changes you have made update the plot and MSWD. You can play with which fit function you like, but generally we utilize the line
	7. When you are happy with your fits, to complete your reduction hit update report table. Once you click the update report table button it will be grayed out which indicates that it is working. Wait until it finishes indicated by the greyed returning to white
	8. Press Save in the bottom left hand corner and then close the window
	
#####New Sample Analysis for ID-TIMS

##Glossary
####Sample-A single collection of a geologic material (usually rock or mineral) from one location. A sample has a lab specific name and a unique identifier such as the IGSN provided by SESAR.
####Project- collection of samples
