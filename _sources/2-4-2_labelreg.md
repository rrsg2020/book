# Image Labeling & Registration

<p style="text-align:justify;">
The  T1 plate of the phantom had 14 spheres that were labeled as the regions-of-interest (ROI) using a numerical mask template created in MATLAB, provided by NIST researchers (Figure 1–a).  To avoid potential edge effects in the T1 maps, the ROI labels were reduced to 60% of the expected sphere diameter. A registration pipeline in Python using the Advanced Normalization Tools (ANTs) (Avants, Tustison, and Song 2009) was developed and shared in the “analysis” repository of our GitHub organization (https://github.com/rrsg2020/analysis, filename: register_t1maps_nist.py). The ROI labels template was nonlinearly registered to each submitted dataset’s T1 map uploaded to OSF.io.
</p>

<b style="text-align:justify;">
Figure 1. ROI selection for the NIST phantom (a) and the human brain (b). a) The 14 ROIs (shades of blue/green) were automatically generated using a script provided by NIST. In yellow are the three reference pins in the phantom, and are not ROIs or spheres. b) ROIs were manually segmented in the human brains in four regions: the genu (yellow, 5x5 voxels), splenium (green, 5x5 voxels), deep gray matter (blue, 5x5 voxels), and cortical gray matter (red, three sets of 3x3 voxels). Note: due to differences in slice positioning from the single-slice datasets provided by certain sites, for some datasets it was not possible to manually segment an ROI in the genu or deep gray matter. In the case of the missing genu, left or right frontal white matter was selected; for deep grey matter, it was omitted entirely for those cases.
</b>

```{image} images/fig1.png
---
width: 500px
name: fig1
align: center
---
```


<p style="text-align:justify;">
Manual ROIs were manually segmented using FSLeyes (McCarthy 2019) in four regions for human datasets (Figure 1-b): genu, splenium, deep gray matter, and cortical gray matter. Automatic segmentation was not used because the data was single-slice and there was inconsistent slice positioning between datasets.
</p>