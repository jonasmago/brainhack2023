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

(todo)=
# My to-do list 
* [X] preprocess the fMRI data with fmriprep
* [X] run GLMs using SPM for the first level and FSL Randomise for the second level 
* [X] replicate GLM in Nilearn 
   * [X] replicate a GLM in Nilearn 
   * [X] compute the correlation between first-level beta maps in the SPM and Nilearn analysis 
   * [ ] replicate the Nilearn GLM with the exact same parameters as in SPM 
      * fd_threshold = 1 (default is 0.5mm)
      * change from `load_confound_strategy` to `load_confound`as it's more custamizable and allows to match parameters of SPM.
      * check if I used a high pass filter in SPM, if not deactivate it in Nilearn.
      * check if I standardized in SPM, if not deactivte it in Nilearn.
   * [ ] Cluster correct the Nilearn second-level contrasts using [`cluster_level-inference`](https://nilearn.github.io/dev/modules/generated/nilearn.glm.cluster_level_inference.html#nilearn.glm.cluster_level_inference).
   * [ ] re-run the GLMs including a brain mask that excludes the cerebellum and brain stem. As we are not interested in the analysis of these regions their exclusion is legit. I can use a mask from brainvolt that I can [download here](https://neurovault.org/collections/6196/).
* [X] connectivity analysis 
   * [X] compute connectome for all conditions and save as `.npy`
   * [ ] compute `graph theory` metrics to characterise and compare the connectomes. François Paugam recommended to look into the [Networks of the Brain](http://www.cs.cmu.edu/~saketn/files/Sporns_Book.pdf) as an introduction.
* [X] compute seed-to-voxel correlations 
* [X] ML classifier 
   * [X] ML classifier on connectomes 
   * [ ] ML classifier on seed-to-voxel maps 
   * [ ] ML classifier on the average activity for each of the 10 trials (not entire runs) cropped to an ROI in the SMA
* [X] Deep Neural Network Decoder using PyTorch