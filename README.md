# CLMRadiomics
Script to compute the features used in the paper "An automatic method
for distinguishing pure histopathological growth patterns of colorectal
liver metastases on CT using deep learning and radiomics: a pilot study .",
M.P.A. Starmans, F. E. Buisman et al. 2020.

## Installation
For the feature extraction, only the PREDICT package, at least version 3.1.5,
and the subsequent dependencies are required, which can be installed through pip:

    pip install "PREDICT>=3.1.5"

For the model optimization, additionally WORC, version 3.2.2, is required:

    pip install "WORC==3.2.2"

## Usage
The ExtractFeatures.py script can be used to extract all features. We provided
you with the exact same configuration file that was used in the study. The
script can be easily modified to use your own data instead of the
provided example data and requires:

1. An image in ITK Image format, e.g. .nii, .nii.gz, .tiff, .nrrd, .raw
2. A segmentation in ITK Image format.
3. Optionally, metadata in DCM format

Extracting the features from the example data should take less than 10 seconds.
Using a larger image and/or mask may result in a longer computation time.

Documentation for the model optimization is provided in the respective script.
