# MS/MS scan pairing
:material-menu-open: **Feature list methods → Processing → Assign MS2 to features**

This module pairs the MS2 fragmentation spectra (collected in [_DDA mode_](../../terminology/general-terminology.md#data-dependent-acqusition-mode-dda)) to the corresponding features, based on the RT offeset between the chromatographic peak and the moment the MS2 was triggered during the run.

!!! warning inline

    This module uses already-resolved feature lists as input; this means that a chromatogram resolving module (e.g. [Local minimum resolver](../featdet_resolver_local_minimum/local-minimum-resolver.md) has to be run first. When processing LC-IMS-MS data, run this mopdule after the IMS resolving step.


---

## Parameters
![MS2 scan pairing](./ms2-scan-pairing.png)

#### Feature lists
Specify the feature list(s) to process.

#### Retention time tolerance
Maximum allowed RT offset between the chromatographic peak and the moment the MS2 was triggered.

#### MS1 to MS2 precursor tolerance (m/z)
Maximum allowed deviation between the _m/z_ associated with the feature, and the precursor _m/z_ the MS2 was triggered for. Being an inter-scan tolerance, we recommend 0.01 m/z and 10 ppm for Orbitrap and TOF instruments.

#### Limit by RT edges
When enabled, the search of MS2 spectra is limited within the start and end time of the feature’s chromatographic peak.

#### Combine MS/MS spectra (TIMS)
When enabled, multiplem MS/MS mobility spectra assigned to a IMS-resolved feature will be merged into a single spectrum.

!!! warning inline

    This is usually not needed. However, if isomers/isobars elute at the same retention time and are close in mobility, the MS/MS window might be larger than the peak in mobility dimension and thus cause chimeric MS/MS spectra.


#### Lock to feature mobility range
When enabled, the search of MS2 spectra in the IMS dimension is limited within the start and end time of the feature’s [mobilogram](../../terminology/ion-mobility-terminology.md#mobilograms).

#### Minimum merged intensity (IMS)
If an ion mobility spectrometry (IMS) feature is processed, this parameter can be used to filter low abundant peaks in the MS/MS spectrum, since multiple MS/MS mobility scans need to be merged together.

---

{{ git_page_authors }}