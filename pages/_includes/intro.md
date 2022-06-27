# Medicare Records FHIR Implementation Guide
<h3>Draft for external review</h3>
<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
* Do not remove this line (it will not be displayed)
{:toc}
<!-- end TOC -->

> <p style="color:#ff0000;">This material is under active development.</p>

## Introduction

This implementation guide is based on [HL7<sup>TM</sup> FHIR<sup>&reg;</sup> Release 3 (STU)](http://hl7.org/fhir/STU3/index.html) and publishes artefacts authored and maintained by the Australian Digital Health Agency to support the electronic exchange of Medicare records between Medicare repositories and the My Health Record system infrastructure in Australia. 

Wherever possible, material in this specification is based on existing standards. All efforts have been made to minimise divergence from the HL7 Australia profiles of HL7 International standards to provide for system interoperability and compatibility with other profiles.

This implementation guide is not to be used as a guide to presentation (or rendering) of the data. It contains no information as to how the data should be displayed and no such guidance should be inferred.

This implementation guide does not describe transport or persistence mechanisms of the resources described by it. API specifications are defined in separate publications.

This implementation guide does not include mappings to another format, for more information see the applicable FHIR resource documentation.
<br/>


## Usage scenarios
[Profiles](profiles.html) in Medicare Records FHIR implementation guide are defined to support the following scenarios:
1. An individual’s Australian Immunisation Register (AIR) records are uploaded to the My Health Record system from a Medicare repository
1. An individual’s Australian Organ Donor Register (AODR) record is uploaded to the My Health Record system from a Medicare repository
1. An individual’s Medicare Benefits Schedule (MBS) records are uploaded to the My Health Record system from a Medicare repository
1. An individual’s Pharmaceutical Benefits Schedule (PBS) records are uploaded to the My Health Record system from a Medicare repository
<br/>


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
            <td>Pre-release at draft for external use. Implemented in FHIR Release 3.0.2 (STU). This version is developed for the Enhanced Use of Immunisations Record Phase 2 and includes support for sending additional immunisation information.
              <ul>
                <li>Added StructureDefinitions: Australian Immunisation Register Immunisation Status, Australian Immunisation Register COVID-19 Immunisation Status, Australian Immunisation Register Immunisation Recommendation, Australian Immunisation Register Notice, Declared Disclaimer, Immunisation Dose Schedule and Vaccine Serial Number</li>
                <li>Amended StructureDefinitions:
                  <ul>
                    <li>Immunization Australian Immunisation Register - amended to represent record of administered vaccination only including new features to represent vaccine serial number and schedule information</li>
                    <li>all StructureDefinitions - updated copyright year and FHIR version </li>
                  </ul>
                </li>
                <li>Removed StructureDefinitions: unused extension Immunisation Cancellation Period</li>
              </ul>
            </td>
        </tr>
        <tr>
            <td>2.1.0</td>
            <td><span style="padding-left: 3px; padding-right: 3px">TBD</span></td>
            <td>TBD. Implemented in FHIR Release 3.0.2 (STU). This version includes changes for the Enhanced Use of Immunisation Records Phase 2 to remove support for the real time immunisation information added in the previous version.
              <ul>
                <li>Amended StructureDefinitions:
                  <ul>
                    <li>Immunization Australian Immunisation Register, and Australian Immunisation Register Notice - removed IHI rules</li>
                    <li>all StructureDefinitions - updated copyright year, date and version</li>
                  </ul>
                </li>  
                <li>Removed StructureDefinitions: Australian Immunisation Register Immunisation Status, Australian Immunisation Register COVID-19 Immunisation Status, Australian Immunisation Register Immunisation Recommendation, Declared Disclaimer, and Immunisation Dose Schedule</li>
                <li>Corrections of editorial nature</li>
              </ul>
            </td>
        </tr>
      </tbody>
</table> 
<br/>


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
        <td>This draft implementation guide has been developed for the Enhanced Use of Immunisation Records Phase 2 project.
            <br/><br/>
            Version 2.1.0 is now available to stakeholders for review however it is not expected to be progressed to publication. 
            <br/><br/>
            It is expected that work on this implementation guide is not going to be progressed until a new project is established. 
        </td>
     </tr> 
     <tr>
       <td>Source material errors</td>
       <td>Material in this specification is based on existing standards and all efforts have been made to minimise divergence. Issues of an editorial nature in the source material (such as spelling or punctuation errors) are intentionally reproduced.</td>
     </tr>
     <tr>
       <td>Non-resolving profile URLs</td>
       <td>Canonical URLs with the prefix of <span style="font-family:courier;">http://ns.electronichealth.net.au/ci/fhir/StructureDefinition/</span> do not resolve. All profiles have an associated <a href="http://hl7.org/fhir/STU3/structuredefinition-definitions.html#StructureDefinition.url">canonical URL</a> that is used to uniquely identify that StructureDefinition (i.e. profile) and is expected to be an address at which that StructureDefinition is (or will be) published. Work is underway to ensure that these URLs resolve or redirect to a meaningful end point in the future.</td>
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
<br/>


