# **Ion mobility raw data overview (LC-IMS-MS)**

## **Description**

:material-menu-open: **Visualization → Ion mobility raw data overview**

The "Ion mobility raw data visualization" module allow a comprehensive navigation of the complex LC-IM-MS raw data. The screenshot belows shows an example of LC-IM-MS data acquired with a Bruker timsTOF instrument:

![im-data-overview](im-data-overview.jpg)

The main window consists of 5 panels and a set of displaying parameters. All the panels are interconnected, which means that moving the cursor in one panel, automatically updates the others. Cursors are displayed as light-blue solid lines in the panels.

## Summed frame spectrum panel [1]

The MS spectrum corresponding to each [frame](../../learners_corner/terminology/ion-mobility-terminology.md#accumulations-mobility-scans-and-frames) is shown in this panel. The displayed MS spectrum is the sum of all the [mobility scans](../../learners_corner/terminology/ion-mobility-terminology.md#accumulations-mobility-scans-and-frames) acquired over that frame (see [Ion mobility spectrometry terminology](../../learners_corner/terminology/ion-mobility-terminology.md)).

## BPC panel [2]

In this panel, the [base peak chromatogram](../../learners_corner/terminology/general-terminology.md#base-peak-chromatogram) is displayed. Each data point corresponds to an individual [frame](../../learners_corner/terminology/ion-mobility-terminology.md#accumulations-mobility-scans-and-frames). Moving the cursor frame-by-frame automatically updateds the 'frame heatmap' and 'summed frame spectrum' panels. Moving the cursor frame-by-frame automatically updateds the 'summed frame spectrum' panels as changing data point in regular LC-MS data would display a different MS scan. Since each frame is made of several [mobily scans](../../learners_corner/terminology/ion-mobility-terminology.md#accumulations-mobility-scans-and-frames), the 'mobilogram chart' and 'frame heatmap' panels automatically updates too.
_Note_. It is currently not possible to display the [TIC chromatogram](../../learners_corner/terminology/general-terminology.md#total-ion-current-chromatogram))

## Mobility scan [3]

[//]: # "Todo Note that this is the only panel that does not possess a cursor as [...]."

## Mobilogram chart [4]

[//]: # "Todo The signal intensity is displayed as a continuous colour scale."

## Frame heatmap [5]

[//]: # "Todo The signal intensity is displayed as a continuous colour scale."

## Ion trace chart [6]

[//]: # "Todo"

## Displaying parameters [6]

**Mobility scan noise level**: This parameter controls the signals shown in the XXX panels (panel n°X). For example, a noise level of 5.0E1 will show only the signals above this value (see below)

[//]: # " TODO SCREENSHOT"

**Frame noise level**: This parameter sets a threshold for the signals shown in the "Summed frame spectrum panel" (panel n°X). Signals from MS spectra acquired over the same frame are summed and shown

**m/z tolerance**

[//]: # "Todo"

**Scan selection**

[//]: # "Todo"

**Retention time width**

[//]: # "Todo"

**Mobilogram bin width (abs)**

[//]: # "Todo"

**EIC/mobilogram ranges**

[//]: # "Todo"
[//]: # "Todo list: - Explain EIC and EIC in mobilogram chart"

{{ git_page_authors }}
