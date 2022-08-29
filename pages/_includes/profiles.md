# {{ page.title }}
{:.no_toc}
<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
* Do not remove this line (it will not be displayed)
{:toc}

## Profiles

The profiles listed below are defined as part of this implementation guide. These profiles make reference to profiles published by HL7 Australia in the [Australian Base Implementation Guide v0.9.3](http://hl7.org.au/fhir/2018Sep/index.html).

###  Australian Immunisation Register record

<table class="list" width="100%">
  <tbody>
   <col width="30%" />
   <col width="70%" />
  <tr>
     <th>Profile</th>
     <th>Description</th>
  </tr>
  <tr>
     <td><a href="StructureDefinition-immunization-air.html">ADHA Australian Immunisation Register Immunization</a></td>
     <td>This profile defines a representation of the record of an administered vaccination, for an individual, held in the Australian Immunisation Register.</td>
  </tr>
   <tr>
      <td><a href="StructureDefinition-flag-air-1.html">ADHA Australian Immunisation Register Flag</a></td>
      <td>This profile defines a representation of an Australian Immunisation Register notice for an individual, e.g. information that an individual has an exemption record or has finished a National Immunisation Program schedule.</td>
   </tr> 
 </tbody>   
</table>
<br/>

### Australian Organ Donor Register record

<table class="list" width="100%">
  <tbody>
     <col width="30%" />
     <col width="70%" />
     <tr>
       <th>Profile</th>
       <th>Description</th>
     </tr>
     <tr>
       <td><a href="StructureDefinition-consent-aodr.html">ADHA Australian Organ Donor Register Consent</a></td>
       <td>This profile defines a representation of donation decision information from the Australian Organ Donor Register.</td>
     </tr>
     <tr>
       <td><a href="StructureDefinition-bodysite-aodr.html">ADHA Australian Organ Donor Register BodySite</a></td>
       <td>This profile defines a representation of an organ or tissue for donation as part of an Australian Organ Donor Register record.</td>
     </tr>
  </tbody>
</table>
<br/>

###  Medicare Benefits Schedule (MBS) claim item record

<table class="list" width="100%">
   <tbody>
      <col width="30%" />
      <col width="70%" />
      <tr>
         <th>Profile</th>
         <th>Description</th>
      </tr>
      <tr>
         <td><a href="StructureDefinition-explanationofbenefit-medicare.html">ADHA Medicare ExplanationOfBenefit</a></td>
         <td>This profile defines a representation of PBS claim items or MBS claim items.</td>
      </tr>
 </tbody>
</table>
<br/>


###  Pharmaceutical Benefits Schedule (PBS) claim item record

<table class="list" width="100%">
   <tbody>
      <col width="30%" />
      <col width="70%" />
      <tr>
         <th>Profile</th>
         <th>Description</th>
      </tr>
      <tr>
         <td><a href="StructureDefinition-explanationofbenefit-medicare.html">ADHA Medicare ExplanationOfBenefit</a></td>
         <td>This profile defines a representation of PBS claim items or MBS claim items.</td>
      </tr>
      <tr>
         <td><a href="StructureDefinition-medicationrequest-pbs.html">ADHA PBS MedicationRequest</a></td>
         <td>This profile defines a representation of prescription data to as part of a PBS claim item.</td>
      </tr>
      <tr>
         <td><a href="StructureDefinition-medication-pbs.html">ADHA PBS Medication</a></td>
         <td>This profile defines a representation of pharmaceutical item data as part of a PBS claim item.</td>
      </tr>
 </tbody>
</table>
<br/>

##  Extensions

The following extensions are defined as part of this implementation guide.

<table class="list" width="100%">
    <tr>
        <th>Extension</th>
        <th>Usage scenario</th>
        <th>Type</th>
        <th>Context</th>
        <th>Profile context</th>
    </tr>
    <tr>
        <td><a href="StructureDefinition-extension-donationdecision.html">Consent Donation Decision</a></td>
        <td>Australian Organ Donor Register record</td>
        <td><a href="http://hl7.org/fhir/STU3/datatypes.html#CodeableConcept">CodeableConcept</a></td>
        <td><a href="http://hl7.org/fhir/STU3/Consent.html">Consent</a></td>
        <td><a href="StructureDefinition-consent-aodr.html">ADHA Australian Organ Donor Register Consent</a></td>
    </tr>
    <tr>
        <td><a href="StructureDefinition-vaccine-serial-number-1.html">Vaccine Vial Serial Number</a></td>
        <td>Australian Immunisation Register record</td>
        <td><a href="http://hl7.org/fhir/STU3/datatypes.html#string">string</a></td>
        <td><a href="http://hl7.org/fhir/STU3/immunization.html">Immunization</a></td>
        <td><a href="StructureDefinition-immunization-air.html">ADHA Australian Immunisation Register Immunization</a></td>
    </tr>
</table>


