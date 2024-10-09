# Light-Dependent Variations in Fatty Acid Profiles and Gene Expression in Antarctic Microalgal Cultures

### Contents
[Overview](#overview)   |   [Research abstract](#abstract)   |   [Script files](#repository-contents)   |   [Metadata examples](#metadata-examples)   |   [R requirements](#r-requirements)
  
## Overview
This repository contains R scripts used to process and analyze fatty acid (FA) percentage data and transcriptomic data for the study:

**Title:** Light-Dependent Variations in Fatty Acid Profiles and Gene Expression in Antarctic Microalgal Cultures  
**Authors:** Jacqui Stuart<sup>1, 2</sup>, Kirsty F. Smith<sup>2</sup>, Matt Miller<sup>2</sup>, John K. Pearman<sup>2</sup>, Natalie Robinson<sup>3</sup>, Lesley Rhodes<sup>2</sup>, Lucy Thompson<sup>2</sup>, Sarah Challenger<sup>2</sup>, Nicole Parnell<sup>4</sup>, Ken G. Ryan<sup>1</sup>  
**Affiliations:**  
1. School of Biological Sciences, Victoria University of Wellington, PO Box 600, Wellington 6140, New Zealand  
2. Cawthron Institute, Private Bag 2, Nelson 7042, New Zealand  
3. National Institute of Water and Atmospheric Research (NIWA), Private Bag 14901, Kilbirnie, Wellington 6241  
4. Lincoln University, 85084 Ellesmere Junction Road, Lincoln 7647  

## Abstract
Photosynthetic eukaryotic microalgae are key primary producers in the sea ice environment. Anticipated changes in sea ice thickness and snow load due to climate change may cause substantial shifts in available light to these ice-associated organisms. This study used a laboratory-based experiment to investigate how light levels, simulating different sea ice thicknesses, affect FA composition in two ice-associated microalgae species: *Nitzschia cf. biundulata* and *Polarella glacialis*. Transcriptomic analyses and fatty acid profiling were used to assess the impact of three light levels:  
- **High light (90 ± 1 μmol photons m⁻² s⁻¹)**: simulating conditions at the bottom of very thin ice  
- **Mid light (10 ± 1 μmol photons m⁻² s⁻¹)**: simulating conditions at the bottom of thin ice  
- **Low light (1.5 ± 1 μmol photons m⁻² s⁻¹)**: simulating conditions at the bottom of thick ice  

The study revealed changes in growth rates and FA composition under different light conditions. *N. cf. biundulata* exhibited significant changes in specific saturated and monounsaturated FAs, with an increase in energy storage-related FAs under conditions mimicking thinner ice. *Polarella glacialis* showed significant changes in polyunsaturated fatty acids (PUFAs), particularly octadecapentaenoic acid (OPA), indicating enhanced membrane fluidity and synthesis of longer-chain PUFAs. Light levels emulating thinning sea ice conditions resulted in down-regulation of photosynthetic genes in *N. cf. biundulata* and up-regulation in *P. glacialis*, indicating diverse acclimation strategies. These findings provide insights into microalgal responses to light stress and potential implications for polar food webs under climate change scenarios.

## Script files
- **scripts/**: R scripts used to process and analyze fatty acid and transcriptomic data.
    - `PhD_Ch6_FattyAcidAnalysis`: Analysis and visualization of fatty acid profiles.
    - `PhD_Ch6_TranscriptomicsAnalysis`: Preprocessing and analysis of transcriptomic data.

## Metadata examples
Below are examples of the .csv data layouts required for each analysis script:

### Fatty Acid Analysis Metadata
![Example of fatty acid analysis data layout](PhD_Ch6_FattyAcidAnalysis_csv-example.png)

### Transcriptomics Analysis Metadata
![Example of transcriptomic analysis data layout](PhD_Ch6_TranscriptomicsAnalysis_metadata-example.png)

## R Requirements
To run the scripts in this repository, you will need:
- **R version >= 4.0**
- **R packages for fatty acid analysis:** `dplyr`, `ggpubr`, `patchwork`, `stringr`, `gridExtra`, `tidyr`
- **R packages for transcriptomic analysis:** `tximport`, `tidyverse`, `DESeq2`, `phyloseq`, `vegan`
