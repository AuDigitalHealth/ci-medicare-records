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

This implementation guide does not describe transport or persistence mechanisms of the resources described by it.

This implementation guide does not include mappings to another format, for more information see the applicable resource documentation in the [FHIR Release 3 (STU) [HL7FHIR3]](#HL7FHIR3).
## Usage Scenarios
The FHIR profiles for each usage scenario are listed below. 
###  Australian Immunisation Register
Profiles that define the representation of vaccination information from the Australian Immunisation Register:
<table class="list" width="100%">
  <tbody>
   <col width="30%" />
   <col width="70%" />
  <tr>
     <th>Profile</th>
     <th>Description</th>
  </tr>
  <tr>
     <td><a href="StructureDefinition-immunization-air.html">Australian Immunisation Register Immunisation</a></td>
     <td>The purpose of this profile is to define a representation of vaccination information from the Australian Immunisation Register (AIR).</td>
  </tr>
  <tr>
      <td><a href="StructureDefinition-flag-air-1.html">Australian Immunisation Register Notice</a></td>
      <td>The purpose of this profile is to define a representation of the Australian Immunisation Register (AIR) notice such as notice an individual has an exemption record or has finished a National Immunisation Program schedule.</td>
  </tr> 
 </tbody>   
</table>
<br/>
###  Pharmaceutical Benefits Schedule (PBS) and Medicare Benefits Schedule (MBS)
Profiles that define representation of Pharmaceutical Benefits Schedule (PBS) claim items or Medicare Benefits Schedule (MBS) claim items:
<table class="list" width="100%">
   <tbody>
      <col width="30%" />
      <col width="70%" />
      <tr>
         <th>Profile</th>
         <th>Description</th>
      </tr>
      <tr>
         <td><a href="StructureDefinition-explanationofbenefit-medicare.html">Explanation of Benefit Medicare</a></td>
         <td>This profile defines a representation of Pharmaceutical Benefits Schedule (PBS) claim items or Medicare Benefits Schedule (MBS) claim items.</td>
      </tr>
      <tr>
         <td><a href="StructureDefinition-medicationrequest-pbs.html">Medication Request Pharmaceutical Benefits Scheme</a></td>
         <td>This profile defines a representation of prescription data to support representation of PBS claim items.</td>
      </tr>
      <tr>
         <td><a href="StructureDefinition-medication-pbs.html">Medication Pharmaceutical Benefits Scheme</a></td>
         <td>This profile defines a representation of pharmaceutical item data to support representation of PBS claim items.</td>
      </tr>
      <tr>
         <td><a href="StructureDefinition-referralrequest-mbsdva.html">Referral Request Medicare Benefits Schedule Department of Veterans’ Affairs</a></td>
         <td>This profile defines a representation of the practitioner that requested the service to support representation of Medicare Benefits Schedule (MBS) claim item records.</td>
       </tr>
 </tbody>
</table>
<br/>
### Australian Organ Donor Register
Profiles that define representation of donation decision information from the Australian Organ Donor Register:
<table class="list" width="100%">
  <tbody>
     <col width="30%" />
     <col width="70%" />
     <tr>
       <th>Profile</th>
       <th>Description</th>
     </tr>
     <tr>
       <td><a href="StructureDefinition-consent-aodr.html">Consent Australian Organ Donor Register </a></td>
       <td>This profile defines a representation of donation decision information from the Australian Organ Donor Register.</td>
     </tr>
     <tr>
       <td><a href="StructureDefinition-bodysite-aodr.html">BodySite Australian Organ Donor Register</a></td>
       <td>This profile defines a representation of organ and tissue details to support representation of Australian Organ Donor Register records.</td>
     </tr>
  </tbody>
</table>


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
            <td>Pre-release at draft for external use. Implemented in FHIR Release 3.0.2 (STU). Added new features for immunisations. Included non-technical corrections from version 1.0.0.</td>
        </tr>
        <tr>
            <td>2.0.1</td>
            <td><span style="padding-left: 3px; padding-right: 3px">TBD</span></td>
            <td>Current draft. Further changes for immunisations.</td>
        </tr>
      </tbody>
</table> 

## Known issues
This table lists known issues with this specification at the time of publishing. We are working on solutions to these issues and encourage comments to help us develop these solutions.

<table class="list" width="100%" cellspacing="6">
    <tbody>
        <tr>
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
        <tr>
            <td>Consent Australian Organ Donor Register</td>
            <td>This profile cannot be used for automated validation.
                <ul>
                    <li>All instances of Consent will fail validation against this profile as nothing can satisfy the required slice category:organDonationConsent. Its use of fixedCodeableConcept does not set discriminator values in a way suitable for slicing.</li>
                    <li>All instances of Consent will fail validation against this profile as nothing can satisfy the implementations of invariants <span style="font-family:courier;">inv-dh-cons-01</span> and <span style="font-family:courier;">inv-dh-cons-02</span>. In the FHIRPath expressions the antecedents are always true, so e.g. an instance with donation-decision of 'permit' and with a specific organ (except.data.reference) will fail with an error against <span style="font-family:courier;">inv-dh-cons-02</span>.</li>
                    <li>Instances of Consent that contain parts of Consent.category:organDonationConsent or Consent.except.action that are intended to be optional, including text and coding.display, will be rejected. Values of CodeableConcepts are set using fixedCodeableConcept, which prohibits parts of CodeableConcept that are intended to be optional, including CodeableConcept.text and CodeableConcept.coding.display.</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>Explanation of Benefit Medicare</td>
            <td>This profile has very limited use for automated validation.
                <ul>
                    <li>Instances of Explanation of Benefit that include medications will fail validation against this profile due to its use of contained resources. In Explanation of Benefit Medicare the element prescription is a contained reference to Medication Request Pharmaceutical Benefits Scheme, which includes a contained reference to Medication Pharmaceutical Benefits Scheme. FHIR does not allow nesting of contained resources.</li>
                    <li>Many true instances of Explanation of Benefit will fail validation against this profile as few things can satisfy the implementations of invariants <span style="font-family:courier;">inv-dh-eob-01</span> and <span style="font-family:courier;">inv-dh-eob-02</span>. In the FHIRPath expressions the antecedents are always true, so e.g. an MBS claim without a prescription instance fails validation.</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>Australian Immunisation Register Immunisation</td>
            <td>This profile has slightly limited use for automated validation.
                <ul>
                    <li>Instances of Immunisation that contain parts of Immunization.vaccinationProtocol.doseStatus that are intended to be optional, including text and coding.display, will be rejected. Values of CodeableConcepts are set using fixedCodeableConcept, which prohibits parts of CodeableConcept that are intended to be optional, including CodeableConcept.text and CodeableConcept.coding.display.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table> 

## References

|[<a name="HL7AUF3B2">HL7AUF3B2</a>]| HL7 Australia, Australian Base Implementation Guide.|
| |[http://hl7.org.au/fhir/2018Sep/index.html](http://hl7.org.au/fhir/2018Sep/index.html)|

|[<a name="HL7FHIR">HL7FHIR</a>]| Health Level Seven, Inc., FHIR - HL7Wiki.|
| |[http://wiki.hl7.org/index.php?title=FHIR](http://wiki.hl7.org/index.php?title=FHIR)|

|[<a name="HL7FHIR3">HL7FHIR3</a>]| Health Level Seven, Inc., 24 October 2019, FHIR Release 3 (STU).|
| |[http://hl7.org/fhir/STU3/](http://hl7.org/fhir/STU3/)|

|[<a name="HL7FHIR4">HL7FHIR4</a>]|Health Level Seven, Inc., 30 October 2019, FHIR R4.|
||[http://hl7.org/fhir/R4/](http://hl7.org/fhir/R4/)|








