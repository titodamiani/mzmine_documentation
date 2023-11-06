# Main window

The MZmine 3 main window consists of four tabs:

![Main window](img/main_window.png)

1.  **Datafiles and feature lists tab**. Here you can find the imported datafiles and
    processed feature lists. Datafiles can be imported in MZmine by drag-and-dropping them directly in the 'MS data files' subtab.

2.  **Main content panel**. [Visualization of raw data](../data_visualization/index.md) as well as [processing results](output.md) (e.g., feature lists) can be done in this panel. Multiple tabs can be opened in this panel. Moreover, tabs can also be opened in separate windows by right-click on the header and 'Open in new window'.

3.  **Menu**. Form the menu you can open/save MZmine projects, change software preferences and access almost any module present in MZmine. Submenus are organized as follows:

    - **Project**. Save/load an MZmine project, open batch mode and set preferences.
    - **Raw data methods**. Modules for spectral processing (e.g., data import/export, mass detection).
    - **Feature detection**. Modules for feature detection and resolving for all supported data types: LC-(IMS)-MS, GC-MS and MS imaging.
    - **Feature lists methods**. Modules for feature lists processing (e.g., isotopes filtering, alignment, spectral deconvolution).
    - **Visualization**. All visualization modules in MZmine for raw data inspection.
    - **Tools**. Modules for various tools (e.g., spectral mirror).
    - **Processing wizard**. Open the [Processing wizard](processing_wizard.md)
    - **Windows**. Modify the [Task overview](#task-overview) position.
    - **Help**. Open [this](https://mzmine.github.io/mzmine_documentation/) documentation, report an issue, etc.

---

## Task overview

The Task overview displays the status/progress of all running tasks. Tasks can be canceled by right click and 'Cancel task'. The task overview can be arranged as a tab in the main content panel, a separate panel in the main window, or simply hidden. To do so, go to '**Windows → Task manager**'.

## Page Contributors

{{ git_page_authors }}
