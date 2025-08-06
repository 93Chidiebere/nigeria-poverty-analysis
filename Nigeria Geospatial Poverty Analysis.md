Nigeria Geospatial Poverty Analysis
This project aims to analyze the relationship between multidimensional poverty and spatial factors in Nigeria using publicly available geospatial data. The analysis focuses on visualizing the spatial distribution of poverty and preparing the data for further investigation into factors like access to education and rural settlements.

Project Stages Completed So Far:
Data Acquisition:

Downloaded administrative boundaries for Nigeria (GADM data) at the state level (gadm41_NGA.gpkg).
Downloaded settlement data for Nigeria (Copernicus data) (nga-pcode-rowca-20150127-2.xlsx). (Note: This file contains information on settlement types and locations, which can be used for spatial analysis.)
Data Loading and Preparation:

Loaded the GADM data into a GeoDataFrame.
Loaded publicly available Multidimensional Poverty Index (MPI) data for Nigerian states from a CSV file (Nigeria_MPI_by_State_2022.csv).
Loaded settlement data from the Copernicus Excel file into a DataFrame.
Merged the GADM state boundaries with the MPI data based on state names.
Prepared settlement data for spatial analysis by filtering for rural settlements and converting coordinates to a suitable geometric format.
Initial Poverty Visualization:

Created a choropleth map of Nigeria showing the MPI for each state to visualize the overall spatial distribution of poverty.
MPI Classification and Individual Map Creation:

Classified Nigerian states into four deprivation groups based on their MPI: Critically Deprived, Severely Deprived, Moderately Deprived, and Minimally Deprived.
Generated individual maps for each of these MPI deprivation groups, highlighting the states within each category and including standard map elements (title, legend, north arrow, scale bar, and MPI definition).
Data Saving to Google Drive:

Implemented code to save the downloaded GADM and Copernicus data files to a specified folder in Google Drive to avoid repeated downloads in future sessions.
Files:
[Your Notebook Name].ipynb: The Jupyter Notebook containing the code for this analysis.
gadm41_NGA.gpkg: Geospatial data for administrative boundaries of Nigeria (downloaded during execution).
Nigeria_MPI_by_State_2022.csv: CSV file containing Multidimensional Poverty Index data by state (uploaded by the user).
nga-pcode-rowca-20150127-2.xlsx: Excel file containing settlement data for Nigeria (downloaded during execution, assuming this was the Copernicus file).
critically_deprived_nigeria_mpi_map.png: Map visualizing critically deprived states by MPI.
severely_deprived_nigeria_mpi_map.png: Map visualizing severely deprived states by MPI.
moderately_deprived_nigeria_mpi_map.png: Map visualizing moderately deprived states by MPI.
minimally_deprived_nigeria_mpi_map.png: Map visualizing minimally deprived states by MPI.
Next Steps (Potential Future Work):
Analyze the relationship between rural poverty rates, out-of-school percentages, and spatial factors (distance to school and proportion of underserved settlements).
Calculate and incorporate out-of-school percentages for all states.
Perform correlation analysis between poverty, out-of-school percentages, and spatial factors.
Visualize the relationships using scatter plots and other suitable visualizations.
Conduct more in-depth spatial analysis using the settlement data.
This README provides a clear overview of the project's progress and can be included in your GitHub repository.