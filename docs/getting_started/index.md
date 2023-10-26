# Getting started

- [Installation](installation.md)
- [Data conversion](data_conversion.md)
- [Batch processing](batch_processing.md)
- [Processing wizard](processing_wizard.md)
  MZmine enables large-scale metabolomics and lipidomics research by
  spectral preprocessing, feature detection, and various options for compound annotation.

![mzmine_workflow](mzmine_workflow.png)

The goal of MS data processing is to turn raw spectral data into a list of detected ions, to estimate their abundance, and to assign chemical annotations based on multiple criteria.

In MZmine, this is done in a three-step approach. First, raw spectral data are centroided and intensity thresholds can be applied to exclude low-intensity signals (e.g. electronic noise) from further processing. The second step is known as feature detection (also ‘feature finding’ or ‘peak picking’) and represents the cornerstone of the processing. A feature can be seen as an m/z signal (more often a group of signals) related to a single metabolite detected during MS analysis. Based on the instrument setup, a feature can be characterised by additional identifiers such as retention time (RT) in chromatography–MS experiments or spatial coordinates in MS imaging data. Untargeted MS experiments typically yield hundreds to thousands of features, although a relatively small portion corresponds to meaningful metabolites detected in the sample. For this reason, the goal of feature detection is to retain all relevant features in the raw spectral data while discarding ‘noisy’ signals. Moreover, features detected in different samples can be aligned to enable consistent sample-to-sample comparison (e.g. statistical analysis). The third and last step of MS data processing in MZmine is feature annotation. Here, various chemical annotations can be assigned to each feature based on additional information retrieved from raw spectral data (e.g. isotope pattern, MS2 spectra), using dedicated modules (e.g. lipid annotation15), or via leveraging the direct integration of MZmine with other popular annotation tools (e.g. SIRIUS16, GNPS17).
