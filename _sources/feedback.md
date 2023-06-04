---
jupytext:
  cell_metadata_filter: -all
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.10.3
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

(feedback)=
# Feedback from the final presentation 
- visualise things in MRIcroGL, soon implemented in nilearn as `niview`
- change my pearson-r values to [-1, 1] (currently [-100,100])
- for comparing nilearn and spm beta maps: specify not-matched. E.g.:
   - between software, within subject, within contrast, within run 
   - between software, between subject, between contrast, between run 
- feature selection must be either on (A) train set or (B) integrated in cross-validation. Make sure it's not selecting featuers on the entier dataset --> danger of overfitting!
- r2 is a measure for the percentage of variance explained. Not relevant here, thus, remove it. 
- explain permutation test for significance testing.
- apply the classifer on beta maps per trials (there are 10 trials per run). I can use ROIs or entire beta masks. The model will take care of the many variables. 
- try a searchlight appraoch: train a classifer on different ROIs or voxels and then compare the accuracy. This could lead to a accuracy map with voxel resolution, however, this is computationally expensive. 
- it's important to  **de-mean** my data before doing this (e.g. use z-score). 
- look into **stratified cross validation** to deal with multiple runs per subject in the classifier. If I use stratification this shouldn't be a problem. 