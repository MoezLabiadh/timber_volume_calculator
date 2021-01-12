# timber_volume_calculator
This script calculates individual tree volumes based on LiDAR derived Canopy Height Module (CHM).

The main Workflow steps:
1) Delineate individual Tree Crowns using Local Maxima and Watershed segmentation algorythms
2) Extract explanatory variables (Tree Height & Crown Area) for each tree
3) Predict DBH using Regression models – from "R.J. Hall et al., 1985: A Comparison of Existing Models for DBH estimation from Large-scale Photos"
4) Estimate Volumes using BC forests 1976 volumes equations).
