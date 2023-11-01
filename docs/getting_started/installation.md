# Installation

The latest version of MZmine 3 can be downloaded from the button below. We provide both installer packages (preferred but might require admin permissions) and portable versions for Windows, macOS and Linux.

[Download MZmine 3 :material-download:](https://github.com/mzmine/mzmine3/releases/latest){ .md-button .md-button--primary }

MZmine comes integrated with _Java Runtime Environment_; therefore, the local _Java_ installation has no impact on MZmine. Windows and macOS users might need to confirm to trust software from an unknown source.

!!! info

    Macos signature was introduced in MZmine version 3.4.0. If you are running older versions, you will need to allow MZmine in the macOS Gatekeeper (see [here](../troubleshooting/macos_sign.md)).

## Set temporary file directory

MZmine can generate a significant amount (several gigabytes) of temporary files during processing. Therefore, we recommend to set the temporary file directory to a local drive (preferably SSD) with enough free space. To do so, go to '**Project → Set preferences → General → Temporary file directory**' and browse the desidered directory. On Windows, old temporary files are deleted when a new MZmine session is started. Changes in the temporary file directory require a restart of the software to take effect.

## Running MZmine

MZmine provides a user-friendly and interactive [GUI](main_window.md) for data exploration, workflow optimization and results validation. Moreover, processing pipelines (including data import/export) can be run with a few clicks using the [batch mode](batch_processing.md). Finally, MZmine can also be run through the [CLI](./batch_processing.md#batch-mode-cli), which enable its integration into fully automated data analysis pipelines (e.g., QC systems).

## Useful resources

If you are new to mass spectrometry data processing in MZmine, checkout the [Learners corner](../learners_corner/index.md) with tutorial videos, webinars and other resources!

New MZmine users can take advantage of the new [_Processing wizard_](processing_wizard.md) for the quick and beginner-friendly generation of data processing workflows for different MS platforms.

{{ git_page_authors }}
