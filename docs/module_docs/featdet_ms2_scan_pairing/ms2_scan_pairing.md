# MS/MS scan pairing
:material-menu-open: **Feature list methods → Processing → Assign MS2 to features**

This module pairs each MS2 fragmentation spectrum (collected in [_DDA mode_](../../terminology/general-terminology.md#data-dependent-acqusition-mode-dda)) to the corresponding feature, based on the RT offeset between the LC peak and the moment the MS2 was triggered during the run. This is crucial to connect the quantitative (i.e., peak area extrapolated from MS1 data) and qualitative information (i.e., annotation based on MS2 spectra) in the LC-(IMS)-MS data. 

!!! warning inline

    This module has to be run on already-resolved feature listes - i.e., a chromatogram resolving module has to be run first. Note: For IM data, run after the IM resolving too. 


---

## Parameters
![MS2 scan pairing](./ms2-scan-pairing.png)

#### Feature lists
Specify the feature lists to process.

#### Retention time tolerance
Maximum allowed offset between the LC peak apex and the RT the MS2 was triggered.

#### MS1 to MS2 precursor tolerance (m/z)
Maximum allowed deviation between the _m/z_ associated with the feature, and the precursor _m/z_ the MS2 was triggered for. We recommend 0.01 m/z and 10 ppm for Orbitrap and TOF instruments.

#### Limit by RT edges
Limit the search of MS2 spectra within the start and end time of the feature’s chromatographic peak. By doing so, the MS2 spectrum will be searched only within the start and end time of the feature’s chromatographic peak.

#### Combine MS/MS spectra (TIMS)
If checked, all MS/MS spectra assigned to a feature will be merged into a single spectrum.

!!! warning inline

    This is usually not needed. However, if isomers/isobars elute at the same retention time and are close in mobility, the MS/MS window might be larger than the peak in mobility dimension and thus cause chimeric MS/MS spectra.


#### Lock to feature mobility range
Add description

#### Minimum merged intensity (IMS)
If an ion mobility spectrometry (IMS) feature is processed, this parameter can be used to filter low abundant peaks in the MS/MS spectrum, since multiple MS/MS mobility scans need to be merged together.

---

{{ git_page_authors }}