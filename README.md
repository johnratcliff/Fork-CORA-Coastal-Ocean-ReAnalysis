README

NOAA’s Coastal Ocean Reanalysis (CORA) provides modeled historical water levels and waves for the Atlantic, Gulf, and Caribbean from 1979-2022. The reanalysis was performed through the partnership of NOAA National Ocean Service (NOS) and University of North Carolina’s (UNC) Institute of Marine Sciences and Renaissance Computing Institute (RENCI). Modeling was performed by ’s  RENCI, and couples ADvanced CIRCulation Model (ADCIRC) and Simulating WAves Nearshore SWAN to produce data points every 300 to 500 meters. Hourly water level observations from NOAA’s Center for Operational Oceanographic Products and Services (CO-OPS) National Water Level Observation Network (NWLON) were both assimilated into modeling, and used for validation of results. This repository hosts Jupyter notebooks to help users access, analyze, and visualize CORA datasets hosted via Amazon Web Services on NOAA’s Open Data Dissemination (NODD) Platform. This repository also hosts code used to produce the reanalysis of the Gulf of Mexico, Atlantic/East Coast, and Caribbean (CORA-GEC), version 1.1. All previous versions (Eg. Version 0.9 used for validation, and version 1.0 used for prototyping) are considered preliminary versions and should be superseded with version 1.1 for operational use. All code is dependent on Python libraries outlined in each notebook. Please ensure you are able to access and install each for optimal performance. 

CORA_Accessing_Data.ipynb
This notebook demonstrates how users can access CORA datasets on NOAA's Open Data Dissemination (NODD) Platform through Amazon Web Services. Model data is extracted  from the nearest model node to a user-specified geographic coordinates and displayed in a timeseries plot. 

CORA_Visualize_Water_Levels.ipynb
This notebook demonstrates how users can access CORA datasets on NOAA's Open Data Dissemination (NODD) Platform through Amazon Web Services and create a 2-dimensional water level surface plot.


CORA_Plot_Mesh
Interested in viewing the bathymetry or mesh that was used in the model to create the CORA data? This notebook allows users to create a rasterized plot of the topobathy at the CORA model nodes and overlay the model mesh.


CORA_Convert_Datums
This notebook allows users to upload a .csv file of extracted CORA time series and run it through NOAA’s Tidal Analysis Datum Calculator (TADC) to convert data from Mean Sea Level (MSL) to other Datums. To run this notebook it will be necessary to also have the Python script and config file for the calculator, which are available on the GitHub repository.


CORA_Compare_Time-Series
This notebook retrieves observed hourly water levels from NWLON stations using CO-OPS Data API to compare with CORA data corresponding to the same location. 


NOAA Open Source Disclaimer
This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project code is provided on an 'as is' basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.

License
Software code created by U.S. Government employees is not subject to copyright in the United States (17 U.S.C. �105). The United States/Department of Commerce reserve all rights to seek and obtain copyright protection in countries other than the United States for Software authored in its entirety by the Department of Commerce. To this end, the Department of Commerce hereby grants to Recipient a royalty-free, nonexclusive license to use, copy, and create derivative works of the Software outside of the United States.
