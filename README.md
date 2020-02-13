# Dual Reporter Pipeline
A pipeline to process dual luciferase assay results.

This R-based workflow is designed to standardize the analysis and publication of dual reporter systems. The main objective is to facilitate calculation and visualization of differential expression between a tested and reference gene. Promega's GloMax luminescence machine produces an excel sheet with expression data for the reporter and the control condition, which will be used as input for the script.

Input data (expressed as arbitrary luminescence units)
* excel sheet containing 2 tables in 96-well lay-out. Technical replicates should be measured in the same well.
* table 1: reporter expression data (firefly)
* table 2: internal control data (renilla)

Data processing
* normalization
* wide --> tidy format
* Fold-change expression


Desired output
 * human readable summary table
    - F/R ratio per condition
    - median or average F/R-values
    - standard deviation

  * visualization options
    - bar graph
    - dotplot with individual data points
    - dotplot + box
    - median to indicate center of measurements
		- selected conditions (x-axis)
    - relative expression normalized to internal control (y-axis)
    - or fold-change relative to reference (y-axis)
