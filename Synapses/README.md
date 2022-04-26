# Gold-Particle-Segmentation

This dataset contains two subfolders:
## “2022 Analyzed Synapses”

10 electron micrographs with immunogold labelled neural tissue. In each Subfolder (e.g. S1, S7, etc.) you will find images and gold particle coordinates for individual samples.<br>

**Main Images:**
1. Raw black and white labelled elecronmicrograph
2.  A colored “mask” indicating the region of interest within the neural tissue for 	i		dentifying gold 	particle locations.
3. A combined EM image with the mask applied.

**Results:**
1. .CSV files and ImageJ ROI files containing the locations of 6nm and 12 nm gold 		particles within 	the images.
2. Images with the particle ROIs overlayed on the original data.

You can treat the “results” data as the ground truth for training your detection/localization 	algorithm, and it should serve as a guide for training your own eyes to identify the structures of i	nterest.

## "2022 Test Data"

Additional examples of freeze fracture replica images with gold particle labelling.  If you find that there is redundancy in the samples, let me know, but these should be useful as additional test data should you need it after training your model.
