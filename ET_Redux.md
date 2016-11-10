##ET_Redux Documentation Overview

ET_Redux is a stand-alone desktop application, produced by CIRDLES.org as the successor to U-Pb_Redux in January, 2015, with the initials "ET" referring to its sponsor [EARTHTIME](http://www.earth-time.org). ET_Redux is cyber infrastructure for geochronologists that automates workflows from sample collection to publicly archiving of results into the NSF-sponsored [Geochron](http://www.geochron.org) community database. ET_Redux exports analysis results as an [aliquot](https://raw.githubusercontent.com/EARTHTIME/Schema/master/AliquotXMLSchema.xsd) XML file, which can be exported to Geochron or stored and shared as desired.  ET_Redux currently serves the ID-TIMS and LAICP-MS U-Pb geochronology communities and is funded 2014 - 2017 by NSF to extend to U-series analyses.

##Information for use of Documentation
The documentation below is essentially a set of step by step instructions on how to operate the software. For auditory and visual learners, youtube video tutorials will be included among the written instructions.

##Concept of operations
ET_Redux provides sophisticated graphical and statistical tools to assist with data ingestion and organization, data reduction, uncertainty propagation, visualizations, publication-ready vectorized tables and plots, and one-click archiving. These include interactive data tables, concordia and weighted mean plots, dynamic decomposition of uncertainties into contributions from individual sources, and algorithms for propagation of systematic uncertainties in tracer calibration and decay constants. 

##Policies that affect the system
ET_Redux is sponsored by EARTHTIME and funded in part by the National Science Foundation under Grant Numbers 0930223 and 1443037. Any opinions, findings and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation (NSF).

##Starting ET_Redux and starting data reduction

##Procedures
(-Youtube videos)

###New Project from Raw Data
1. Open ET_Redux - note that this will generate two html files, ChangeLog.html and Credits.html
1. To start, click "Project" in the top left corner.
1. Then click "New Project" from Raw Data.
1. Click "LA-ICP-MS".  Note that IDTIMS raw data is currently processed by our software [Tripoli](http://cirdles.org/projects/tripoli/).
1. Now you will see the Project Manager interface where you specify your project. Start by entering your Project Name and then choosing the appropriate:
  * File Handling Protocol
  * Raw Data Template
  * Analysis Purpose
1. Finally, click "Prepare to load/Process Raw Data." Then, depending on your file handling protocol you will be able to select your data file or data folder and then click "Open" to show the parameters manager. If you use folders, be sure that all necessary files are present.
1. Confirm that all parameters are correct - the defaults are shown initially.
1. Full Uncertainty propagation is the default - use the fast option to explore datasets only.
1. Select your Primary Reference Material.  Note the default is set in the Lab Settings Manager.
1. Now you are ready to start the reduction process. You can either start a live session while the mass spectrometer is producing data or proceed to reduce an already-collected dataset as explained below.

####Live Data Reduction Processing:
1. Click "Save and Monitor/Process Raw Data"
1. Once the live data monitor is launched you will have to wait for at least 3-4 analysis to be recorded by the mass spectrometer software and processed by ET_Redux before seeing any data.
1. To reject an analysis, right click on the selected fraction name in the report table located in the bottom portion of the manager and it will be sent to the rejected fractions tab but will still be reduced.
1. To look at individual samples (Reference Materials or Unknowns), double click on the project name in the panel to the left of the concordia, and a drop down menu will show all available groups to view on Concordia and on the PDF.  Note that the reference materials both primary and secondary will not appear in the PDF view.
1. To set filters for percent discordance and percent uncertainty, adjust the sliders in the panel under the PDF. To apply them to the Concordia plot, select "apply filters" checkbox under the Concordia.  To set the sliders to the default values specified in the lab data manager, click "Default", and to clear the filters, click "Clear".
1. To change what dates are shown on the PDF, select one of the three dates (6/8, 6/7, or best date). We suggest the best date option.
1. Best date filter can be changed while you are looking at unknowns in Concordia space by sliding the blue best date handle on the vertical axis.
1. When a fraction is removed be patient as it will take until the next primary reference material fraction to update the session.
1. If you need to refresh, click "Refresh Views"
1. Wait until the run has completed and proceed to Project Raw Data Manager (see below).

####Project Raw Data Manager
1. Consider using the following view options singly or in combination to explore your data:
  * Y-axis Scaling set to Independent
  * Show All Local Y-axis
  * Make horizonal zoom very tight to highlight patterns in data
1. Start with the default "Intercept" method tab.
1. Review the reference materials to make sure ratios are within acceptable rages. It will be very clear when an analysis is bad. You will either see a very large scatter in data points or the fit line will be far off the data points.  Be sure to select the appropriate fit functions on a ratio-by-ratio basis, or even for each graph.
1. Click "Show Session" button.
1. The time-based session views for each ratio plot the reference materials and their 1-sigma absolute uncertainties in black and over-dispersion of uncertainties in red, if calculated. Each session can be fitted with a choice of mean, line, exponential or spline functions. 
1. To remove a data point for a reference material, hover over the black dot and right click. You will be asked to “exclude this fraction", click on it and the black dot will change to red indicating it has been removed.
1. Once you have removed all unwanted data points you MUST click "Refit" on the left update the plot and MSWD. 
1. Next, click "Fit Unknowns" and evaluate each fraction and ratio for the unknowns and the secondary reference materials, which are also treated as unkowns.
1. When you are happy with your fits, to complete your reduction click "Update Report Table", which will remain grayed out until it finishes and then returns to the color white.
1. Return to the main window showing the data table and click "Sample Dates" in the bottom right to launch the sample date manager with the concordia, weighted means, and PDF plots and views.
	
###New Sample Analysis for ID-TIMS (needs work)
1. At the main menu, click "Sample" and then click "New Sample Analysis for ID-TIMS" to launch the ID-TIMS Workflow Manager for ANALYSIS MODE of a Sample.  You can always return to this window by clicking the "Manage Sample" menu item under the main emanu "Sample".
1. Provide the "Local Sample Name" and "IGSN".  SESAR is the default registry to date.
1. Select the "Analysis Purpose" and  the "Phsyical Constants Model".
1. For each aliquot, provide the name and then click "Add Name" to add the aliquot to the left-hand list.  Once this list is populated with the names of the aliquots, clicking each name sets up the next step of either manually "inserting fractions" or "importing a folder of fractions", which consists of XML files produced by Tripoli or similar software.  These XML files must conform to the schema found [here](https://raw.githubusercontent.com/EARTHTIME/Schema/master/UPbReduxInputXMLSchema.xsd).
1. Fractions and aliquots may be removed using the appropriate buttons.  If importing is done, the default fraction should be removed.
1. For each fraction of each aliquot complete the entries in the interactive data table at the bottom of the window.
1. For manual update, Click "Close and Save" button.
1. For Live Workflow, be sure to set the following parameters before clicking "Close and Save" button.
  * one
  * two
  * three
  

##Glossary (needs work - has two definitions of Sample)
####Aliquot- phsyical pieces of a sample whose dates you wish to interpret seperately.
####Fraction- a paired U+Pb analysis
####Live Workflow- establishes a direct link between Tripoli (another CIRDLES software product) and ET_Redux.
####Project- collection of samples
####Sample-A single collection of a geologic material (usually rock or mineral) from one location. A sample has a lab specific name and a unique identifier such as the IGSN provided by SESAR. It is composed of aliquots or physical pieces of the sample.
