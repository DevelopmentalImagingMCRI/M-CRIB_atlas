# M-CRIB atlas 

## Files available here include:

* T2- and T1-weighted templates
* Hard segmentation images
* Structure probability maps
* Segmentation label files

T2- and T1-weighted templates are based on the 10 M-CRIB participants, constructed with ANTS using nonlinear symmetric diffeomorphic normalisation (SyN) as the transformation model. Further details are available in the paper referred to below.

Thresholded hard segmentation images were constructed by registering the 10 parcellations to the T2-weighted template, and selecting the most frequently occurring label across the sample at each voxel. These segmentations have been thresholded in increments of 0.1 probability. Thus, for an image thresholded at 0.7, the given label in any voxel was present in at least 7 of the 10 participants. Sub-threshold voxels have a value of 0. For (effectively) unthresholded hard segmentation, please use the image labeled '0.1'. 

Individual structure probability maps are based on registration of binarised labels for each structure for the 10 participants to the T2-weighted M-CRIB template.

Label files in ITK and FreeSurfer formats list structure indices, names, RGB and alpha values. 


Templates and hard segmentations based on rigid and affine registration are also available, purely for the purpose of further illustrating the variability in morphology in the M-CRIB sample. However, these will produce suboptimal labeling, so are not recommended for this purpose. These are available in the current repository under the branch 'linear\_atlas\_versions'. To access this, 

```bash
git checkout linear_atlas_versions
```
Images are in the subfolder linear\_M-CRIB\_atlas\_versions


If available, we may add further M-CRIB atlas data via this page.

Please cite [this paper](http://www.sciencedirect.com/science/article/pii/S1053811916305444) when using and referring to the M-CRIB atlas.


