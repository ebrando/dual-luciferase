# Dual Reporter 
A pipeline to process dual reporter assay results.

# Overview
This R-based workflow is designed to standardize the analysis and publication of dual reporter systems, such as Promega's Dual Luciferase Reporter assay. 

The pipeline produces the following parameters in a human readable table: 
* Normalized expression to internal control (F/R ratio)
* average expression per condition

Results can be plotted as individual datapoints per conditions, including the average. 

x-axis: conditions.

y-axis: 
* relative reporter expression normalized to internal control (renilla) 
* fold-change reporter expression normalized to empty vector 
