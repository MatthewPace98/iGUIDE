## iGUIDE - improved Genome-wide Unbiased Identification of Double-strand DNA break Events
[![Build Status](https://travis-ci.org/cnobles/iGUIDE.svg?branch=master)](https://travis-ci.org/cnobles/iGUIDE)
[![CircleCI](https://circleci.com/gh/cnobles/iGUIDE.svg?style=svg)](https://circleci.com/gh/cnobles/iGUIDE)
[![Documentation Status](https://readthedocs.org/projects/iguide/badge/?version=latest)](http://iguide.readthedocs.io/en/latest/?badge=latest)
[![DOI](https://zenodo.org/badge/88088016.svg)](https://zenodo.org/badge/latestdoi/88088016)


Bioinformatic pipeline for processing iGUIDE and GUIDE-seq samples.

### Description
iGUIDE is a pipeline written in [snakemake](http://snakemake.readthedocs.io/) for processing and analyzing double-strand DNA break events. These events may be induced, such as by designer nucleases like Cas9, or spontaneous, as produced through DNA replication or ionizing radiation. A laboratory bench-side protocol accompanies this software pipeline, and can be found [**https://doi.org/10.1186/s13059-019-1625-3**](https://doi.org/10.1186/s13059-019-1625-3). 

To get started, checkout the iGUIDE documentation at [iGUIDE.ReadTheDocs.io](https://iguide.readthedocs.io/).

### Changelog:

**v1.1.0 (February ??, 2019)**

* Modified how samples designated as Mock are treated during the analysis
* Mock samples can now be indicated by "None" or "Control" as well 
  (case-insensitive)
* Updated standard report template to display more relevant information at the 
  beginning, included the combinations table
* Abundance can now be selected as [Read], [UMI], or [Fragment]{default} within 
  config parameters

**v1.0.0 (August 15th, 2019)**

* Release of version 1.0.0!!!
* iGUIDE is a computational pipeline that supports the detection of DSBs induced
  by designer nucleases
* Aligner support for BLAT and BWA currently implemented, let us know if you 
  would like to see others.
* Flexible pipeline processing built on Snakemake, supports a binning system
  to better distribute workflow for whichever system it is being processed on
* Documentation supporting a Quickstart and User Guide hosted by [ReadTheDocs](https://iguide.readthedocs.io/)
