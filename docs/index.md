# Welcome to the MZmine 3 wiki!

MZmine 3 is an open-source, platform-independent software for mass spectrometry data
processing and visualization. Here you can find documentation for both processing and visualization modules in MZmine 3. Moreover,
data processing pipelines for untargeted [LC-MS](workflows/lcmsworkflow/lcms-workflow.md)
and [LC-IMS-MS](workflows/imsworkflow/ion-mobility-data-processing-workflow.md) feature detection
are described and general recommendations are given. New to MZmine 3? [Get started](./getting_started/index.md)!

!!! note ""

    When using the MZmine software, please cite the following paper:<br>
    Robin Schmid, Steffen Heuckeroth, Ansgar Korf et al. Integrative analysis of multimodal mass spectrometry data in MZmine 3. _**Nature Biotechnology**_ (2023), DOI: [10.1038/s41587-023-01690-2](https://www.nature.com/articles/s41587-023-01690-2).

---

# About MZmine 3

Since the introduction of MZmine 2 in 2010, the [MZmine project](https://github.com/mzmine) has matured into a community-driven, highly
collaborative platform and. Over the years, MZmine's functions have expanded based on users' needs and feedback and, thanks to the invaluable contribution of [developers](https://github.com/mzmine/mzmine3/graphs/contributors) from all around the world, MZmine has become one of the most popular tools for untargeted MS data analysis and visualization.

Compared to MZmine 2, MZmine 3 comes with a redesigned and fully customizable [GUI](getting_started/main-window-overview.md) based on the JavaFX technology that allows an interactive visualization and validation of the results at every processing step. A completely new data structure provides the flexibility to process any type of mass spectrometry data,
like LC-MS, GC-MS and MS-imaging. Moreover, MZmine 3 supports ion mobility, with a
dedicated [LC-IM-MS data visualization](visualization_modules/ims_raw_data_overview/IM-data-visualisation.md)
module and [feature detection workflow](workflows/imsworkflow/ion-mobility-data-processing-workflow.md). Finally, significant effort was devoted to trace memory issues and bottlenecks, resulting in an unprecendent processing performance and scalability.

Thanks to community efforts and collaboration with other open-source projects, the MZmine ecosystem is tightly integrated with popular third-party
software for MS data analysis, such as
the [SIRIUS](https://bio.informatik.uni-jena.de/software/sirius/) suite for _in silico_ metabolite
annotation, the [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp?redirect=auth)
platform, the [MetaboAnalyst](https://www.metaboanalyst.ca/)
web app for univariate and multivariate statistical anlysis, _etc._

!!! tip "**COMING SOON!**"

    We are implementing the [Mass Spec Query Langauge](https://github.com/rformassspectrometry/SpectraQL) (MassQL) to explore your MS data with human-readable, succinct queries! The project is suppported by the [Google Summer of Code](https://summerofcode.withgoogle.com/) program..

---

## How to contribute

You can contribute by improving existing modules or even adding new featurs to MZmine 3. Please, check out our
brief [tutorial](http://mzmine.github.io/development.html). You can also contribute to this wiki and help new users to get started with MZmine 3.
See [here](contribute/contribute.md) how to contribute to the documentation.

{{ git_page_authors }}
