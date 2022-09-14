# {{ page.title }}
{:.no_toc}
<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
* Do not remove this line (it will not be displayed)
{:toc}
<!-- end TOC -->


## Introduction

The Australian Digital Health Agency Medicare Records FHIR Implementation Guide contains HL7™ FHIR® Release 3 (STU3) artefacts authored and maintained by the Agency to support the electronic exchange of Medicare records between Medicare repositories and the My Health Record system infrastructure in Australia. 

Wherever possible, material in this specification is based on existing standards. All efforts have been made to minimise divergence from the HL7 Australia profiles of HL7 International standards to provide for system interoperability and compatibility with other profiles.


## Scope

This guide is scoped to the FHIR conformance artefacts (i.e. [Profiles and Extensions](profiles.html)) that define the data structure of FHIR resources to support the following scenarios:
1. An individual’s Australian Immunisation Register (AIR) record is uploaded to the My Health Record system from a Medicare repository
1. An individual’s Australian Organ Donor Register record is uploaded to the My Health Record system from a Medicare repository
1. An individual’s Medicare Benefits Schedule (MBS) claim item records are uploaded to the My Health Record system from a Medicare repository
1. An individual’s Pharmaceutical Benefits Schedule (PBS) claim item records are uploaded to the My Health Record system from a Medicare repository

This guide, including the profiles defined, is intended to support interactions between individuals, healthcare providers, the My Health Record system, and other clinical information systems.

The FHIR conformance artefacts are published in an Agency FHIR NPM package for use with FHIR and FHIR-aware tools. 

The FHIR package contains the validation form (JSON + SCH) of the conformance artefacts for direct use in validation operations and example resource instances that demonstrate use cases and conformance requirements. This release of the implementation guide is scoped to the content of the Agency FHIR NPM package v1.0.0 and is provided to assist readers and users in understanding the content of that package.  


## How to read this guide

This guide is divided into several pages which are listed at the top of each page in the menu bar.

- [Home](index.html): This page provides the introduction and scope for this guide.
- [Profiles and Extensions](profiles.html): This page lists the set of profiles and extensions that are defined in this guide to exchange quality data. Each profile page includes a narrative description and guidance, formal definition and the expectations for must support elements in each profile. Although the guidance typically focuses on the profiled elements, it may also may focus on un-profiled elements to aid with implementation.
- [Downloads](downloads.html): This page provides links to downloadable artefacts including the Agency FHIR NPM package.
- [Disclaimers](disclaimers.html): This page lists the licensing, copyright, and disclaimers under which this guide is issued. 
- [Change Log](changes.html): This page documents the changes across versions of this implementation guide.

