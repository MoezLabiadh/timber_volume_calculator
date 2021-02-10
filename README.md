# Timber Volume Calculator
## Description
This model calculates individual tree volumes based on LiDAR derived Canopy Height Module (CHM).

## Workflow
The main Workflow steps:
1) Delineate individual Tree Crowns using Local Maxima and Watershed segmentation algorythms
2) Extract explanatory variables (Tree Height & Crown Area) for each tree
3) Predict DBH using Regression models – from "R.J. Hall et al., 1985: A Comparison of Existing Models for DBH estimation from Large-scale Photos"
4) Estimate Volumes using BC forests 1976 volumes equations).


## Required packages
The following packages need to be installed on your Python Env to run the this code:
- Numpy
- Scipy
- Pandas
- Osgeo (gdal and ogr)
- Scikit-iame

```Python
import os
import sys

from osgeo import gdal,ogr,osr

import math
import numpy as np
import pandas as pd
from scipy import ndimage as ndi

from skimage.feature import peak_local_max
from skimage.morphology import watershed
from skimage.measure import regionprops,regionprops_table

import matplotlib.pyplot as plt
%matplotlib inline 
```

## Calculate CHM



## Contributions
All contributions are welcome.
