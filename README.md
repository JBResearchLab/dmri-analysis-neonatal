### dMRI pipeline for neonatal data (PRENCOG and TEBC)
These folders have the scripts for running the neonatal dMRI analysis pipeline, written in python and bash:

* Converting from raw DICOMS to data in BIDS specification
* Preprocessing using [FSL](https://fsl.fmrib.ox.ac.uk/fsl/docs/#/), [ANTs](https://stnava.github.io/ANTs/), [MRtrix3](https://mrtrix.readthedocs.io/en/latest/#), [designer](https://nyu-diffusionmri.github.io/DESIGNER-v2/) and [iBeat2](https://github.com/iBEAT-V2/iBEAT-V2.0-Docker)
  * The pipeline processes structural and diffusion MRI to generate:
	* Separating brain from skull, brain tissue segmentation and parcellation, spatial normalization
	* Confound estimation
* Motion estimation for data exclusion
* First-level modeling
   * Contrast generation
   * Splithalf functionality (i.e., analyse full or half runs)
   * Adult ROI timecourse regression
* Timecourse extraction
* Second-level modeling

See the Wiki page for more detailed information about running each step of the pipeline.
