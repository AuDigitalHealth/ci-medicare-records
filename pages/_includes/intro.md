# {{ site.data.fhir.igName }} FHIR Implementation Guide
<h3>Draft for restricted external review</h3>
<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
* Do not remove this line (it will not be displayed)
{:toc}
<!-- end TOC -->

## Introduction

This implementation guide is an HL7<sup>TM</sup> FHIR<sup>&reg;</sup> specification to represent Medicare information for the My Health Record system and related applications.

This [implementation guide](http://hl7.org/fhir/STU3/implementationguide.html#scope) is based on [FHIR Release 3 (STU) [HL7FHIR3]](#HL7FHIR3).

This implementation guide is not to be used as a guide to presentation (or rendering) of the data. It contains no information as to how the data described by it should be displayed and no such guidance should be inferred.

This implementation guide does not describe transport or persistence mechanisms of the resources described by it. The repository gateway and API specification are defined in separate publications.

This implementation guide does not include mappings to another format, for more information see the applicable resource documentation in the [FHIR Release 3 (STU) [HL7FHIR3]](#HL7FHIR3).

## Usage scenarios
The Medicare Records FHIR implementation guide is defined to support the following scenarios:
* An individual’s Australian Immunisation Register (AIR) records are uploaded to the My Health Record system from a Medicare Repository
* An individual’s Australian Organ Donor Register (AODR) record is uploaded to the My Health Record system from a Medicare Repository
* An individual’s Pharmaceutical Benefits Schedule (PBS) records are uploaded to the My Health Record system from a Medicare Repository
* An individual’s Medicare Benefits Schedule (MBS) records are uploaded to the My Health Record system from a Medicare Repository

The profiles for each usage scenario are listed on the [Profiles](profiles.html) page.

## Editorial note
This implementation guide is an early working specification that is available for comment and review. It may be used to solicit feedback and to provide insight as to the expected content in a forthcoming stable and approved version of the specification.

This implementation guide may not be considered to be complete enough or sufficiently reviewed to be safe for implementation and use in production systems. It may have known issues and still be in development.

## Document Information

### Key Information

<table class="list" width="100%" cellspacing="6">
    <tbody>
        <tr>
            <td><b>Owner</b></td>
            <td>Director, Connectivity and Informatics</td>
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
            <td>Initial release at approved for external use. Implemented in FHIR Release 3 (STU).</td>
        </tr>
        <tr>
            <td>2.0.0</td>
            <td><span style="padding-left: 3px; padding-right: 3px">27 Nov 2020</span></td>
            <td>Pre-release at draft for external use. Implemented in FHIR Release 3.0.2 (STU). This version is developed for the Enhanced Use of Immunisations Record Phase 2 and includes support for sending additional immunisation information via FHIR bundle from Services Australia to the My Health Record system.
            <br/><br/>
            Added structure definitions: Australian Immunisation Register Immunisation Status, Australian Immunisation Register COVID-19 Immunisation Status, Australian Immunisation Register Immunisation Recommendation, Australian Immunisation Register Notice, Declared Disclaimer, Immunisation Dose Schedule and Vaccine Serial Number.
            <br/><br/>
            Ammended Immunization Australian Immunisation Register to represent record of administered vaccination only including new features to represent vaccine serial number and schedule information.
            <br/><br/>
            Removed unused Immunisation Cancellation Period extension.</td>
        </tr>
        <tr>
            <td>2.1.0</td>
            <td><span style="padding-left: 3px; padding-right: 3px">TBD</span></td>
            <td>Current draft. Implemented in FHIR Release 3.0.2 (STU). This version includes changes for the Enhanced Use of Immunisation Records Phase 2 to remove support for the real time immunisation information obtained from Services Australia via newly established intergration service.
             <br/><br/>
             Removed structure definitions: Australian Immunisation Register Immunisation Status, Australian Immunisation Register COVID-19 Immunisation Status, Australian Immunisation Register Immunisation Recommendation, Declared Disclaimer, and Immunisation Dose Schedule.
             <br/><br/>
             Made minor informative changes to all remaining profiles.</td>
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
        <td>Medicare Records FHIR implementation guide roadmap</td>
        <td>This draft implementation guide has been developed for the Enhanced Use of Immunisation Records Phase 2 project included in MHR Release 12 29 April 2021.
        <br/><br/>
        ....
        </td>
     </tr> 
     <tr>
       <td>Source material errors</td>
       <td>Material in this specification is based on existing standards and all efforts have been made to minimise divergence. Issues of an editorial nature in the source material (such as spelling or punctuation errors) are intentionally reproduced.</td>
     </tr>
     <tr>
       <td>Non-resolving profile URLs</td>
       <td>Canonical URLs with the prefix of <span style="font-family:courier;">http://ns.electronichealth.net.au/ci/fhir/StructureDefinition/</span> do not resolve. All profiles have an associated <a href="http://hl7.org/fhir/STU3/structuredefinition-definitions.html#StructureDefinition.url">canonical URL</a> that is used to uniquely identify that structure definition (i.e. profile) and is expected to be an address at which that structure definition is (or will be) published. Work is underway to ensure that these URLs resolve or redirect to a meaningful end point in the future.</td>
     </tr>
     <tr>
       <td><a href="StructureDefinition-consent-aodr.html">Consent Australian Organ Donor Register </a></td>
       <td>Normative defects; behaves as a failure case. All instances of Consent will fail validation against this profile.
         <ul>
           <li>cannot satisfy the required slice category:organDonationConsent. See <a href="https://github.com/AuDigitalHealth/ci-medicare-records/issues/6"> ci-medicare-records/issues/6</a>.</li>
           <li>cannot satisfy invariants inv-dh-cons-01 and inv-dh-cons-02. See <a href="https://github.com/AuDigitalHealth/ci-medicare-records/issues/5"> ci-medicare-records/issues/5</a>.</li>
           <li>cannot include parts of category:organDonationConsent or except.action that are intended to be optional, including text and coding.display. See <a href="https://github.com/AuDigitalHealth/ci-medicare-records/issues/2"> ci-medicare-records/issues/2</a>.</li>
         </ul>
       </td>
     </tr>
     <tr>
       <td><a href="StructureDefinition-explanationofbenefit-medicare.html">Explanation of Benefit Medicare</a></td>
       <td>Normative defects; unintended failure cases.
         <ul>
           <li>cannot include prescriptions; failure caused by nested contained resources. See <a href="https://github.com/AuDigitalHealth/ci-medicare-records/issues/3"> ci-medicare-records/issues/3</a>. </li>
           <li>Additional unintended failure cases due to definition of inv-dh-eob-01, inv-dh-eob-02 and inv-dh-eob-04. See <a href="https://github.com/AuDigitalHealth/ci-medicare-records/issues/4"> ci-medicare-records/issues/4</a>. </li>
         </ul>
       </td>
     </tr>
  </tbody>
</table> 

## References

|[<a name="HL7AUF3B2">HL7AUF3B2</a>]| HL7 Australia, 12 September 2018, Australian Base Implementation Guide, Version 0.9.3.|
| |[http://hl7.org.au/fhir/2018Sep/index.html](http://hl7.org.au/fhir/2018Sep/index.html)|

|[<a name="HL7FHIR">HL7FHIR</a>]| Health Level Seven, Inc., FHIR - HL7Wiki.|
| |[http://wiki.hl7.org/index.php?title=FHIR](http://wiki.hl7.org/index.php?title=FHIR)|

|[<a name="HL7FHIR3">HL7FHIR3</a>]| Health Level Seven, Inc., 24 October 2019, FHIR Release 3 (STU).|
| |[http://hl7.org/fhir/STU3/](http://hl7.org/fhir/STU3/)|

|[<a name="HL7FHIR4">HL7FHIR4</a>]|Health Level Seven, Inc., 30 October 2019, FHIR R4.|
||[http://hl7.org/fhir/R4/](http://hl7.org/fhir/R4/)|








