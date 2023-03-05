# Fitting Model and Pipeline

<p style="text-align:justify;">
A reduced-dimension non-linear least squares (RD-NLS) approach was used to fit the complex general inversion recovery signal equation: 
</p>

```{math}
:label: my_label
S(TI) = a + be^{-TI/T_1}
```

<p style="text-align:justify;">
where a and b are complex constants. This approach, introduced in (Barral et al. 2010), models the general T1 signal equation without approximating for a very long TR. The a and b constants inherently factor TR in them. Barral et al. shared the implementation of their fitting algorithm used in their paper. To facilitate its use in our pipelines, we used a wrapper around this code available in the open-source software qMRLab (Cabana et al. 2015; Karakuzu et al. 2020), which provides a standardized API to call the fitting in MATLAB/Octave scripts.
</p>

<p style="text-align:justify;">
A Jupyter Notebook data processing pipeline was written using MATLAB/Octave. This pipeline automatically downloads all the datasets, loads each dataset configuration file, fits the T1 data voxel-wise, and exports the resulting T1 map to the NIfTI and PNG formats for quality assurance. This pipeline is available in a GitHub repository (https://github.com/rrsg2020/t1_fitting_pipeline, filename: RRSG_T1_fitting.ipynb). Once all submissions were collected and the pipeline was executed, the T1 maps were uploaded to OSF.io.
</p>