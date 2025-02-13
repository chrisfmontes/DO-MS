---
layout: default
title: Home
nav_order: 1
description: "DO-MS: Modular and extensible visualization of mass-spec data"
permalink: /
---

# **DO-MS**
{: .fs-9 }

<u>D</u>ata-Driven <u>O</u>ptimization of <u>M</u>ass <u>S</u>pectrometry Methods
{: .fs-6 .fw-300}

![Python Package](https://github.com/SlavovLab/DO-MS-DIA/actions/workflows/python-package.yml/badge.svg)
![GitHub release](https://img.shields.io/github/release/SlavovLab/DO-MS.svg)
![GitHub](https://img.shields.io/github/license/SlavovLab/DO-MS.svg)

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Download](https://github.com/SlavovLab/DO-MS/releases/latest){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [BioArxiv Preprint](https://www.biorxiv.org/content/10.1101/2023.02.02.526809v1){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 } [GitHub Repository](https://github.com/SlavovLab/DO-MS){: .btn .fs-5 .mb-4 .mb-md-0 }

![]({{site.baseurl}}/assets/images/do-ms-dia_title_v2.png){: width="90%" .center-image}

## Aim of DO-MS
The performance of ultrasensitive liquid chromatography and tandem mass spectrometry (LC-MS/MS) methods, such as [single-cell proteomics by mass spectrometry](https://scope2.slavovlab.net/mass-spec/sensitive-mass-spectrometry-analysis) and [multiplexed data-independent acquisition experiments](https://plexdia.slavovlab.net/), depends on multiple interdependent parameters. This interdependence makes it challenging to specifically pinpoint the sources of problems in the LC-MS/MS methods. 

This applies to data-dependent acquisition (DDA) as well as to data-indepent acquisition (DIA) experiments. For example, a low signal at the MS2 level in a DDA experiment can be due to poor LC separation, ionization, apex targeting, ion transfer, or ion detection. DO-MS aims to specifically diagnose such problems by interactively visualizing data from all levels of bottom-up LC-MS/MS analysis.

### Installation

Install this application by downloading it from the [release page](https://github.com/SlavovLab/DO-MS/releases/latest) and by following the [installation instructions]({{site.baseurl}}/docs/installation).


## Getting Started
Please read our detailed getting started guides:
* [Getting started with DIA preprocessing]({{site.baseurl}}/docs/getting-started-preprocessing)
* [Getting started with DIA reports]({{site.baseurl}}/docs/getting-started-dia-app)
* [Getting started with DDA reports]({{site.baseurl}}/docs/getting-started-dda-app)


### Requirements
This application has been tested on R >= 3.5.0, OSX 10.14 / Windows 7/8/10/11. R can be downloaded from the main [R Project page](https://www.r-project.org/) or downloaded with the [RStudio Application](https://www.rstudio.com/products/rstudio/download/). All modules are maintained for MaxQuant >= 1.6.0.16 and DIA-NN > 1.8.1.

The application suffers from visual glitches when displayed on unsupported older browsers (such as IE9 commonly packaged with RStudio on Windows). Please use IE >= 11, Firefox, or Chrome for the best user experience.

### Running the Interactive Application

The easiest way to run the app is directly through RStudio, by opening the `DO-MS.Rproj` Rproject file

![]({{site.baseurl}}/assets/images/do-ms-proj.png){: width="70%" .center-image}

and clicking the "Run App" button at the top of the application, after opening the `server.R` file. We recommend checking the "Run External" option to open the application in your default browser instead of the RStudio Viewer.

![]({{site.baseurl}}/assets/images/do-ms-run.png){: width="70%" .center-image}

You can also start the application by running the `start_server.R` script.

### Customization

DO-MS is designed to be easily user-customizable for in-house proteomics workflows. Please see [Building Your Own Modules]({{site.baseurl}}/docs/build-your-own) for more details.

### Hosting as a Server

Please see [Hosting as a Server]({{site.baseurl}}/docs/hosting-as-server) for more details.

### Supporting other Search Engines

This application is currently maintained for (MaxQuant)[https://www.nature.com/articles/nbt.1511] >= 1.6.0.16 and  (DIA-NN)[https://www.nature.com/articles/s41592-019-0638-x] >= 1.8. Adapting to other search engines is possible but not provided out-of-the-box. Please see [Integrating Other Search Engines ]({{site.baseurl}}/docs/other-search-engines) for more details.

### Can I use this for Metabolomics, Lipidomics, etc... ?

While the base library of modules are based around bottom-up proteomics by LC-MS/MS, this project is fundamentally compatible with _any delimited text files_ (CSV, TSV, etc). These implementations will require some programming work, but once it is done DO-MS gives you a extensible framework that can be used over-and-over again to generate shareable reports. See [Integrating Other Search Engines ]({{site.baseurl}}/docs/other-search-engines) for more details

------------

## About the project

The manuscript for this tool is published at the Journal of Proteome Research: [https://pubs.acs.org/doi/10.1021/acs.jproteome.9b00039](https://pubs.acs.org/doi/10.1021/acs.jproteome.9b00039)
The manuscript for the extended version 2.0 can be found on bioArxiv: [https://www.biorxiv.org/content/10.1101/2023.02.02.526809v1](https://www.biorxiv.org/content/10.1101/2023.02.02.526809v1)

Contact the authors by email: [nslavov\{at\}northeastern.edu](mailto:nslavov@northeastern.edu).

### License

DO-MS is distributed by an [MIT license]({{site.github_link}}/blob/master/LICENSE).

### Contributing

Please feel free to contribute to this project by opening an issue or pull request in the [GitHub repository]({{site.github_link}}).

-------------

## Help!

For any bugs, questions, or feature requests,
please use the [GitHub issue system](https://github.com/SlavovLab/DO-MS/issues) to contact the developers.
