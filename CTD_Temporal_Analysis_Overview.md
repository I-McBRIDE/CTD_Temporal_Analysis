## Temporal Analysis of the Straight of Juan de Fuca Water Column
#### By: Ian McBride

### Goals:
* How does the water column in an estuarine enviornment develope over the course of a year?
* Can we make an easily interpretable time series that plots the different variables of a CTD cast over a 12 month period?

### Motivations:
* CTD analysis is commonly only performed spatially. Often researchers want to know how the water column changes as distance increases from the freshwater input. The CTD casts are taken once at multiple points, plotted separately, and compared.   
* Plotting CTD data as a time series will provide new insights into how the water column changes dynamically through time. This data could then be used in conjunction with a time series of planktonic species abundance to better understand the ecology of species. 

### Data:
* My CTD data was compiled from the Washington State Department of Ecology. The data is available in one-month chunks on their webpage, linked below. The individual pieces were copied directly from their webpage and compiled into a single CSV file within excel. The CSV file containing twelve months is then imported into the python code. 
* [Environmental Information Management System](https://apps.ecology.wa.gov/eim/search/SMP/MarineAmbientSingleStationOverview.aspx?FocusTab=True&ResultType=MarineAmbientProfile&StudyMonitoringProgramUserId=MarineAmbient&StudyMonitoringProgramUserIdSearchType=Equals&LocationUserIds=SJF000&LocationUserIdSearchType=Equals&LocationUserIDAliasSearchFlag=True&FieldActivityDateRangeBeginning=12%2F1%2F2017%2012%3A00%3A00%20AM&FieldActivityDateRangeEnding=12%2F31%2F2017%2012%3A00%3A00%20AM)

### Analysis Methods:
* The crux of the data analysis involved converting the one-dimensional CSV columns into two-dimensional data arrays suitable for contour plotting. This involved creating a series for the parameter of interest and assigning that data to a multi-index. For example, Salinity is indexed to depth and date to coordinate each value in space and time. These series could then be converted into a data array and plotted as a contour map.
* Additionally, I calculate the summer and winter mean for each variable in terms of depth to visualize the contrasting water columns. To do this, I extract the four summer months (May, June, July, and August) and the four winter months (December, January, February, and March) from the data array of the parameter of interest. These means are plotted together in a simple line graph.

### Conclusions:
* I hypothesize that the finalized figures produced unexpected results due to the strong currents characteristic of the sample location. For example, the bottom waters of the sample location were substantially fresher and warmer in the winter than in the summer. This may have interesting impacts on the ecology of benthic organisms in the area and may warrant future investigations. 

### References:
* Washington State Department of Ecology, Marine Water and Sediment Monitering Program