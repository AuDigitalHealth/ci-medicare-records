# Medicare Records FHIR Implementation Guide
<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
* Do not remove this line (it will not be displayed)
{:toc}
<!-- end TOC -->

<p style="color:#DAA520;">Draft for external review</p>

## Introduction

This implementation guide is based on [HL7<sup>TM</sup> FHIR<sup>&reg;</sup> Release 3 (STU)](http://hl7.org/fhir/STU3/index.html) and publishes artefacts authored and maintained by the Australian Digital Health Agency to support the electronic exchange of Medicare records between Medicare repositories and the My Health Record system infrastructure in Australia. 

Wherever possible, material in this specification is based on existing standards. All efforts have been made to minimise divergence from the HL7 Australia profiles of HL7 International standards to provide for system interoperability and compatibility with other profiles.

This implementation guide, including the profiles defined, are not designed to support interactions between individuals, healthcare providers, the MHR system, and other clinical information systems. One or more separate publications define interactions for each system endpoint.

This implementation guide does not include mappings to another format, for more information see the applicable FHIR resource documentation.
<br/><br/>

## Usage scenarios
[Profiles](profiles.html) in Medicare Records FHIR implementation guide are defined to support the following scenarios:
1. An individual’s Australian Immunisation Register (AIR) record is uploaded to the My Health Record system from a Medicare repository
1. An individual’s Australian Organ Donor Register record is uploaded to the My Health Record system from a Medicare repository
1. An individual’s Medicare Benefits Schedule (MBS) claim item records are uploaded to the My Health Record system from a Medicare repository
1. An individual’s Pharmaceutical Benefits Schedule (PBS) claim item records are uploaded to the My Health Record system from a Medicare repository
<br/><br/>


## Key information

<table class="list" width="100%" cellspacing="6">
    <tbody>
        <tr>
            <td><b>Owner</b></td>
            <td>Director, Interoperability Products</td>
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
<br/>


### Product version history

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
            <td>Pre-release for review. Implemented in FHIR Release 3.0.2 (STU). This version is developed for the enhanced use of immunisation records.
              <br/><br/>Added:
                  <ul>
                    <li>profile Australian Immunisation Register Immunisation Status</li>
                    <li>profile Australian Immunisation Register COVID-19 Immunisation Status</li>
                    <li>profile Australian Immunisation Register Notice</li>
                    <li>profile Australian Immunisation Register Immunisation Recommendation</li>
                    <li>profile Declared Disclaimer</li>
                    <li>extension Immunisation Dose Schedule</li>
                    <li>extension Vaccine Serial Number</li>
                  </ul>
                Amended:
                  <ul>
                    <li>profile Australian Immunisation Register Immunisation - corrected to represent only administered vaccines, added vaccine serial number and schedule information</li>
                  </ul>
                Removed: 
                  <ul>
                    <li>extension Immunisation Cancellation Period</li>
                  </ul>
            </td>
        </tr>
        <tr>
            <td>2.1.0</td>
            <td><span style="padding-left: 3px; padding-right: 3px">**IN PROGRESS**</span></td>
            <td>**PROGRESSING THROUGH ASSURANCE**<br/><br/>Implemented in FHIR Release 3.0.2 (STU). This version includes addresses changes in implementation scope.
              <br/><br/>Amended:
                  <ul>
                    <li>Australian Immunisation Register Immunisation - removed constraints on population of Immunization.patient.identifier</li>
                    <li>Australian Immunisation Register Notice - removed constraints on population of Flag.subject.identifier</li>
                    <li>Consent Australian Organ Donor Register - corrected category slicing <a href="https://github.com/AuDigitalHealth/ci-medicare-records/issues/6">ci-medicare-records #6</a>, corrected FHIRPath for inv-dh-cons-01 & inv-dh-cons-02 <a href="https://github.com/AuDigitalHealth/ci-medicare-records/issues/5">ci-medicare-records #5</a>, corrected Consent.except.action to patternCodeableConcept <a href="https://github.com/AuDigitalHealth/ci-medicare-records/issues/2">ci-medicare-records #2</a></li>
                    <li>Explanation of Benefit Medicare - corrected FHIRPath for inv-dh-eob-01, inv-dh-eob-02 & inv-dh-eob-04 <a href="https://github.com/AuDigitalHealth/ci-medicare-records/issues/4">ci-medicare-records #4</a></li>
                  </ul> 
                Removed:
                <ul>
                    <li>profile Australian Immunisation Register Immunisation Status</li>
                    <li>profile Australian Immunisation Register COVID-19 Immunisation Status</li>
                    <li>profile Australian Immunisation Register Immunisation Recommendation</li>
                    <li>profile Declared Disclaimer</li>
                    <li>extension Immunisation Dose Schedule</li>
              </ul>
            </td>
        </tr>
      </tbody>
</table> 
<br/>









