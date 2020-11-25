# {{ site.data.fhir.igName }} FHIR Implementation Guide
<h3>Draft for external review</h3>
<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
* Do not remove this line (it will not be displayed)
{:toc}
<!-- end TOC -->

## Introduction

This implementation guide is an HL7<sup>TM</sup> FHIR<sup>&reg;</sup> specification to represent structured Medicare information for the My Health Record system and related applications.

This [implementation guide](http://hl7.org/fhir/STU3/implementationguide.html#scope) is based on [FHIR Release 3 (STU) [HL7FHIR3]](#HL7FHIR3).

## Document purpose and scope
The primary aim of this implementation guide is to support the transmission of structured information from Medicare systems to the My Health Record system.

This implementation guide is not to be used as a guide to presentation (or rendering) of the data. It contains no information as to how the data described by it should be displayed and no such guidance should be inferred.

This implementation guide does not describe transport or persistence mechanisms of the resources described by it.

Reference has been made to International and Australian Standards, and to Standards from Health Level Seven. The following standards are referred to in the text in such a way that some or all of its content constitutes requirements for the purposes of this specification:
* [FHIR Release 3 (STU) [HL7FHIR3]](#HL7FHIR3)
* [Australian Base Implementation Guide (AU Base 1.1.1) [HL7AUF3B2]](#HL7AUF3B2)

Wherever possible, material in this specification is based on existing standards. Issues of an editorial nature in the source material (such as spelling or punctuation errors) are intentionally reproduced.


## Profiles
The FHIR profiles that form part of this implementation guide are shown below. The profiles described in this implementation guide do not include profile-specific mappings to another format as part of their description. The base FHIR STU3 mapping content for each of the resources referenced in this implementation guide can be found on the applicable resource documentation in the [FHIR Release 3 (STU) [HL7FHIR3]](#HL7FHIR3).

Profiles that define the representation of vaccination information from the Australian Immunisation Register:
* [Australian Immunisation Register Immunisation Status](StructureDefinition-observation-airimmstatus-1.html)
* [Australian Immunisation Register COVID-19 Immunisation Status](StructureDefinition-observation-aircovid19immstatus-1.html)
* [Immunization Australian Immunisation Register](StructureDefinition-immunization-air.html)
* [Australian Immunisation Register Immunisation Recommendation](StructureDefinition-immunizationrecommendation-air-1.html)
* [Australian Immunisation Register Notice](StructureDefinition-flag-air-1.html)
* [Declared Disclaimer](StructureDefinition-basic-decldiscl-1.html)

Profiles that define representation of Pharmaceutical Benefits Schedule (PBS) claim items or Medicare Benefits Schedule (MBS) claim items:
* [Explanation of Benefit Medicare](StructureDefinition-explanationofbenefit-medicare.html)
* [Medication Request Pharmaceutical Benefits Scheme](StructureDefinition-medicationrequest-pbs.html)
* [Medication Pharmaceutical Benefits Scheme](StructureDefinition-medication-pbs.html)
* [Referral Request Medicare Benefits Schedule Department of Veterans’ Affairs](StructureDefinition-referralrequest-mbsdva.html)

Profiles that define representation of donation decision information from the Australian Organ Donor Register:
* [Consent Australian Organ Donor Register](StructureDefinition-consent-aodr.html)
* [BodySite Australian Organ Donor Register](StructureDefinition-bodysite-aodr.html)


## Editorial note
This implementation guide is an early working specification that is available for comment and review. It may be used to solicit feedback and to provide insight as to the expected content in a forthcoming stable and approved version of the specification.

This implementation guide may not be considered to be complete enough or sufficiently reviewed to be safe for implementation and use in production systems. It may have known issues and still be in development.


## Intended audience
This implementation guide is aimed at software development teams, architects, designers, clinicians and informatics researchers who are responsible for the delivery of clinical applications, infrastructure components and messaging interfaces, and also for those who wish to evaluate the clinical suitability of the Agency-endorsed specifications.

This implementation guide and related artefacts are technical in nature and the audience is expected to be familiar with the language of health data specifications and to have some familiarity with health information standards and specifications, such as [HL7 FHIR [HL7FHIR3]](#HL7FHIR3) and Standards Australia IT-014 documents. Definitions and examples are provided to clarify relevant terminology usage and intent.

## Document Information

### Key Information

<table class="list" width="100%" cellspacing="6">
    <tbody>
        <tr>
            <td><b>Owner</b></td>
            <td>National Health Chief Information Officer, Infrastructure Operations</td>
        </tr>
        <tr>
            <td><b>Contact for enquiries</b></td>
            <td>
                <p>Australian Digital Health Agency Help Centre <br />
                t:   1300 901 001<br />
                e:  <a href ="mailto:help@digitalhealth.gov.au">help@digitalhealth.gov.au</a></p>    
            </td>
        </tr>
    </tbody>
</table> 

### Product Version History
<table class="list" width="100%" cellspacing="6">
	<col style="width:15%"/>
	<col style="width:15%"/>
	<col style="width:70%"/>
    <tbody>
        <tr>
            <th>Product version</th>
            <th>Date</th>
            <th>Release comments</th>
        </tr>
        <tr>
            <td>1.0.0</td>
            <td><span style="padding-left: 3px; padding-right: 3px">1 Nov 2018</span></td>
            <td>Initial public release at approved for external trial use. Implemented in FHIR Release 3 (STU).</td>
        </tr>
        <tr>
            <td>2.0.0</td>
            <td><span style="padding-left: 3px; padding-right: 3px">?? 2020</span></td>
            <td>Release at draft. Implemented in FHIR Release 3.0.2 (STU).<br/>This version includes new features for immunisations. </td>
        </tr>
      </tbody>
</table> 

## Known issues
This table lists known issues with this specification at the time of publishing. We are working on solutions to these issues and encourage comments to help us develop these solutions.

<table border="1" cellpadding="1" valign="middle">
<tbody>
  <tr bgcolor="#DCDCDC">
    <th>Reference</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Source material errors</td>
    <td>Material in this specification is based on existing standards and all efforts have been made to minimise divergence. Issues of an editorial nature in the source material (such as spelling or punctuation errors) are intentionally reproduced.</td>
  </tr>
  <tr>
    <td>Non-resolving profile URLs</td>
    <td>Canonical URLs with the prefix of <span style="font-family:courier;">http://ns.electronichealth.net.au/ci/fhir/StructureDefinition/</span> do not resolve. All profiles have an associated <a href="http://hl7.org/fhir/STU3/structuredefinition-definitions.html#StructureDefinition.url">canonical URL</a> that is used to uniquely identify that structure definition (i.e. profile) and is expected to be an address at which that structure definition is (or will be) published. Work is underway to ensure that these URLs resolve or redirect to a meaningful end point in the future.</td>
  </tr>
 </tbody>
</table> 

## References

|[<a name="HL7AUF3B2">HL7AUF3B2</a>]| HL7 Australia, Australian Base Implementation Guide (AU Base 1.1.1), build version 1.1.1 21 January 2020.|
| |[http://hl7.org.au/fhir/base/aubase1.1/index.html](http://hl7.org.au/fhir/base/aubase1.1/index.html)|

|[<a name="HL7CDAR2">HL7CDAR2</a>]|Health Level Seven, Inc., January 2010, HL7 Clinical Document Architecture, Release 2.|
| |[http://www.hl7.org/implement/standards/product_brief.cfm?product_id=7](http://www.hl7.org/implement/standards/product_brief.cfm?product_id=7)|

|[<a name="HL7FHIR">HL7FHIR</a>]| Health Level Seven, Inc., FHIR - HL7Wiki, accessed 2 October 2019.|
| |[http://wiki.hl7.org/index.php?title=FHIR](http://wiki.hl7.org/index.php?title=FHIR)|

|[<a name="HL7FHIR3">HL7FHIR3</a>]| Health Level Seven, Inc., 24 October 2019, FHIR Release 3 (STU).|
| |[http://hl7.org/fhir/STU3/](http://hl7.org/fhir/STU3/)|

|[<a name="HL7FHIR4">HL7FHIR4</a>]|Health Level Seven, Inc., 30 October 2019, FHIR R4.|
||[http://hl7.org/fhir/R4/](http://hl7.org/fhir/R4/)|








