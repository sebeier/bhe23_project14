---
title: 'BioHackEU23 report: Enabling continuous RDM using Annotated Research Contexts with RO-Crate profiles for ISA'
title_short: 'BioHackEU23 #14: RO-Crate profile for ARC/ISA'
tags:
  - research data management
  - continuous integration
  - ARC
  - ISA
  - RO-Crate
  - Bioschemas
authors:
  - name: Sebastian Beier
    orcid: 0000-0002-2177-8781
    affiliation: 1
  - name: Timo Mühlhaus
    orcid: 0000-0003-3925-6778
    affiliation: 2
  - name: Cyril Pommier
    orcid: 0000-0002-9040-8733
    affiliation: 3
  - name: Stuart Owen
    orcid: 0000-0003-2130-0865
    affiliation: 4
  - name: Dominik Brilhaus
    orcid: 0000-0001-9021-3197
    affiliation: 5
  - name: Heinrich Lukas Weil
    orcid: 0000-0003-1945-6342
    affiliation: 2
  - name: Florian Wetzels
    orcid: 0000-0002-5526-7138
    affilation: 2
  - name: Gavin Chait
    orcid: 0000-0003-3733-6299
    affilation: 6
  - name: Daniel Arend
    orcid: 0000-0002-2455-5938
    affilation: 7
  - name: Manuel Feser
    orcid: 0000-0001-6546-1818
    affilation: 7
  - name: Gajendra Doniparthi
    orcid: 0009-0005-5417-2275
    affilation: 2
affiliations:
  - name: Forschungszentrum Juelich, CEPLAS, BioSC, Institute of Bio- and Geosciences, IBG4 Bioniformatics, 52428 Juelich, Germany
    index: 1
  - name: RPTU Kaiserslautern-Landau, Germany
    index: 2
  - name: Université Paris-Saclay, INRAE, URGI, France
    index: 3
  - name: Department of Computer Science, The University of Manchester, United Kingdom
    index: 4
  - name: Cluster of Excellence on Plant Sciences (CEPLAS) / Heinrich-Heine-University Düsseldorf, Germany
    index: 5
  - name: Whythawk, Oxford, United Kingdom
    index: 6
  - name: Leibniz Institute for Plant Genetics and Crop Plant Research (IPK) Gatersleben, Germany
    index: 7
date: 8 November 2023
cito-bibliography: paper.bib
event: BH23EU
biohackathon_name: "BioHackathon Europe 2023"
biohackathon_url:   "https://biohackathon-europe.org/"
biohackathon_location: "Barcelona, Spain, 2023"
group: Project 14
# URL to project git repo --- should contain the actual paper.md:
git_url: https://github.com/sebeier/bhe23_project14
# This is the short authors description that is used at the
# bottom of the generated paper (typically the first two authors):
authors_short: Sebastian Beier \emph{et al.}
---


# Introduction

As part of the BioHackathon Europe 2023, we here report on the plan this group had initially as well as the deviations from said plan during the event. 

## Description of Project 14

A prevailing paradigm in Research Data Management (RDM) is to publish research datasets in designated archives upon conclusion of a research process. However, it is beneficial to abandon the notion of ""final"" or ""static"" data artifacts and instead adopt a continuous approach towards working with research data, where data is constantly archived, versioned, and updated. This ""immutable yet evolving"" perspective allows for the application of existing technologies and processes from software engineering, such as continuous integration, release practices, and version management backed by decades of experience, and adaptable to RDM.

To facilitate this, we propose the Annotated Research Context (ARC), a data and metadata layout convention based on the well-established ISA model for metadata annotation and implemented as Git repositories. ARCs are amenable towards frequent, lightweight data management operations, such as (meta)data validation and transformation. The Omnipy Python library is designed to help develop stepwise validated (meta)data transformations as scalable data flows that can be incrementally designed, updated, and rerun as requirements or data evolve.

To demonstrate the concept of ""continuous RDM"" we will use Omnipy to define and orchestrate Git-backed CI/CD (Continuous Integration/Continuous Delivery) data flows to convert ISA metadata present in ARCs into validated RO-Crate representations adhering to the Bioschemas convention. A RO-Crate package combines the actual research data with its metadata description. Downstream, this allows semantic interpretation by Galaxy for e.g. workflow execution as well as machine-readable data access and data harvesting for search engines such as FAIDARE.

## Work Plan

Overview about the intended work plan:

1. Generate Bioschemas representation of the ISA model
2. Specify formal RO-Crate Profile for ISA
3. Extend existing CI/CD workflow for ARC/ISA using Omnipy and whyqd
4. (Bonus objective: Finalise MIAPPE to ISA-JSON mapping)

# Results

Actual results produced during discussions, modelling and implementations during the BioHackathon Europe 2023.

## Changes from the original work plan

Any deviations from the work plan

## Bioschemas

![Conceptional view of the duality of LabProcess and LabProtocol from a ISA-model perspective](./LabProtocol_LabProcess.png)

## RO-Crate Profile

## ISA to MIAPPE 

## Crosswalks from ISA to GEO using whyqd

# Discussion

...

## Acknowledgements

...

## References
