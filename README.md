# Intercalation Analysis
Scripts for time-lapse analysis of  biological experiments.
The 2 scripts are for data analysis of the results obtained from ImageJ automated quantificaiton.
(see https://github.com/federicosaltarin/intercalation_fiji_macro)

The Mege Summaries script combines different single CSV file in a single one containing all the results from all the timepoints in all the movies. Using REGEX on the first column, it extracts well and FOV information (from the multi-well acquisition we acquire in different wells and 6 FOV per well). From a table defined by the user it gets and add the information abou the experimental condition. In the end it saves the final CSV, ready for analysis.

Analysis and plotting of the results is then done with the Script Intercalation file. Plotting is done per fov (possible to check technical consistency of data) and then per condition to compare experimental conditions. 
Main representation is for the time series: number or area of diplacement events over time represented by smoothed curves or boxplots.

The 2 notebooks require this libraries:

- dplyr
- data.table
- stringr
- tcltk
- ggplot2
- tcltk
