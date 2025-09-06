# Pansharpening-Brovey-PCA
This is a Remote Sensing Project that pansharpens satellite image subsets using two pansharpening techniques: Brovey Transform and Principle Component Analysis (PCA).

# Definition & Importance
Pansharpening combines high-resolution panchromatic (PAN) images with lower-resolution multispectral (MS) images to produce a single high-resolution color image.

Why is it Important?

Improved Spatial Resolution: Enhances image clarity for better analysis and interpretation.

Enhanced Decision-Making: Supports environmental monitoring, land classification, and urban planning.

Cost-Effective: Utilizes existing satellite data to achieve high-resolution imagery.

# How It's Made
Coding Languages/libraries: Python, GDAL, Matplotlib, NumPy, sklearn

Data Supported: Landsat 9 Imagery, Bands 2 (blue),3 (green), 4(red) and 8(panchromatic)

Steps Taken:
1) Conversion to TOA Reflectance
   
    Purpose: To correct atmospheric effects and calibrate the image.
3) Resampling from 30m to 15m
   
    Method: Bilinear interpolation, using the weighted average of the 4 nearest pixels.
   
    Outcome: Improved spatial resolution for better analysis.
5) Create a 500 x 500 pixel subset
   
   Outcome: Optimization of Brovey and PCA (working on a smaller data set)
7) Apply Brovey Transform on the 500 x 500 pixel subset
8) Apply PCA on the 500 x 500 pixel subset

# Known Issues
If this code is run in Google Colab it is possible that the MTL file will disapear 

You may see bluish streaks due to the conversion of Digital Numbers to TOA

<img width="750" height="361" alt="image" src="https://github.com/user-attachments/assets/b4aeef8b-0f89-4ae9-8e3d-ea61ed6fbd15" />

<img width="758" height="358" alt="image" src="https://github.com/user-attachments/assets/1dd9c64e-6302-4024-8a2e-9876575c0bad" />


