### dMRI pipeline for neonatal data (PRENCOG and TEBC)
These folders have the scripts for running the neonatal dMRI analysis pipeline, written in python and bash:

* Converting from raw DICOMS to data in BIDS specification
* Preprocessing using [FSL](https://fsl.fmrib.ox.ac.uk/fsl/docs/#/), [ANTs](https://stnava.github.io/ANTs/), [MRtrix3](https://mrtrix.readthedocs.io/en/latest/#), [designer](https://nyu-diffusionmri.github.io/DESIGNER-v2/) and [iBeat2](https://github.com/iBEAT-V2/iBEAT-V2.0-Docker)
  * The pipeline processes structural and diffusion MRI to generate:
	* Separating brain from skull, brain tissue segmentation and parcellation, spatial normalization to different spaces and alignment between diffusion and structural images
	* Will perform the following processing to the diffusion images: denoising; correction for gibbs rings artifacts; eddy current, head movement and EPI distortion correction; and B0 bias field inhomogeneity correction. 
* Several maps for the diffusion are obtained afterwards:
   * DTI
   * DKI
   * NODDI: NODDI, personalized NODDI, modulated NODDI and modulated personalized NODDI
   * BedpostX
   * Xtract!
   * SMT: microscopic diffusion tensor and multi-compartment microscopic diffusion

See the Wiki page for more detailed information about running each step of the pipeline.
