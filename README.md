# LeadingModes_rfMRI
This repository contains data and codes for the following manuscript:

**Leading Basic Modes of Spontaneous Activity Drive Individual Functional Connectivity Organization in the Resting Human Brain**

Xi Chen et al., (2023)

## Fold Data
- Fold Figure1
  - Fold REST1

    Brain maps of leading basic modes for REST1 of the HCP dataset.
  -	Fold REST2

   	Brain maps of leading basic modes for REST2 of the HCP dataset.
  -	Weights_REST1_REST2.mat

   	Weights of the first 30 basic modes for two runs (i.e., REST1 and REST2 of the HCP dataset). 
  -	System_level_fluctuation_amplitude.mat

   	System-level fluctuation amplitudes for leading basic modes.
  -	Similar_REST1_REST2.mat

   	Spatial similarity of the first ten basic modes between two runs (i.e., REST1 and REST2).

- Fold Figure2
  -	NeuroSynth_term_corr.xlsx
  
    Correlations between leading basic modes and cognitive terms obtained based on the NeuroSynth meta-analytic database<sup>1</sup>.
  -	Similar_CognitiveComponent.mat

   	Correlations between leading basic modes and 12 cognitive components derived from Yeo et al<sup>2</sup>.

- Fold Figure3
  -	FC_original.mat
  
    Original functional connectivity matrix for REST1 of the HCP dataset (group level).
  -	Fold FC_each_mode
  
    Functional connectivity patterns corresponding to five leading basic modes (REST1 of the HCP dataset)
  -	Fold FC_reconst_group

   	Reconstructed functional connectivity matrices obtained by using different numbers of basic modes (1~5) based on the theoretical modeling (group level).
  -	Similarity_Reconst_Original_individual.mat
  
    Spatial similarity between reconstructed and original FC matrices at the individual level for both runs. The reconstructed FCs were obtained by using different numbers of basic modes (1~10).
  -	Fold Similarity_Reconst_between_runs_individual
  
    Intra- and inter-subject similarity of reconstructed FC matrices between two runs. The reconstructed FCs were obtained by using different numbers of basic modes (1~10).
  -	Identification_Accuracy_Idiff.mat
  
    Individual identification accuracy and differential identifiability Idiff based on the reconstructed FC matrix.

- Fold Figure4	
  -	Fold RW
  
    Brain maps of leading basic modes at rested wakefulness state in the sleep-deprivation dataset.
  -	Fold SD
  
    Brain maps of leading basic modes after sleep-deprivation in the sleep-deprivation dataset.
  -	Weights_RW_SD.mat
  
    Weights of the first 30 basic modes at rested wakefulness state and after sleep-deprivation in the sleep-deprivation dataset.
  -	Similar_RW_REST1.mat
  
    Spatial similarity of the first ten basic modes between rested wakefulness state in the sleep-deprivation dataset and REST1 of HCP dataset.
  -	Similar_RW_SD.mat
  
    Spatial similarity between the first ten basic modes between rested wakefulness state and after sleep-deprivation in the sleep-deprivation dataset.
  -	SD-RW.nii
  
    Brain map of the regions showing significant changes after sleep-deprivation (p <0.05, FDR corrected). Regional differences in fluctuation amplitudes are displayed.
  -	Coactivation_pattern_and_changes.mat
  
    System-level coactivation patterns for basic mode 1 at rested wakefulness and after sleep-deprivation, and between-state differences.

- Fold Parcellations
  - This fold contains parcellations<sup>3</sup> used in the manuscript.

## Fold Code
- Mode_extract.m
 
  Basicmode identification.
- get_leading_number.py

  Identification of leading basic modes.
- reconst_FC.m

  Functional connectivity reconstruction.

## References
1. Yarkoni T, Poldrack RA, Nichols TE, Van Essen DC, Wager TD. Large-scale automated synthesis of human functional neuroimaging data. Nat. Methods 8, 665-670 (2011).
2. Yeo BT, et al. Functional specialization and flexibility in human association cortex. Cereb. Cortex 25, 3654-3672 (2015).
3. Schaefer A, et al. (2018) Local-Global Parcellation of the Human Cerebral Cortex from Intrinsic Functional Connectivity MRI. Cereb Cortex 28(9):3095-3114.
