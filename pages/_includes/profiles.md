# {{ page.title }}
The [profiles](http://hl7.org/fhir/STU3/profiling.html) listed below are defined as part of this implementation guide. HL7 Australia base profiles referenced by this implementation guide can be found in [Australian Base Implementation Guide [HL7AUF3B2]](index.html#HL7FHIR3).

###  Australian Immunisation Register record

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
     <td>This profiles defines a representation of the record of an administered vaccination, for an individual, held in the Australian Immunisation Register (AIR).</td>
  </tr>
   <tr>
      <td><a href="StructureDefinition-flag-air-1.html">Australian Immunisation Register Notice</a></td>
      <td>This profile defines a representation of an Australian Immunisation Register (AIR) notice for an individual. A notice may include information that an individual has an exemption record or has finished a National Immunisation Program schedule.</td>
   </tr> 
 </tbody>   
</table>
<br/>

### Australian Organ Donor Register record

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
       <td>This profile defines a representation of an organ or tissue for donation as part of an Australian Organ Donor Register record.</td>
     </tr>
  </tbody>
</table>

###  Medicare Benefits Schedule (MBS) claim item record

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
         <td><a href="StructureDefinition-referralrequest-mbsdva.html">Referral Request Medicare Benefits Schedule Department of Veterans’ Affairs</a></td>
         <td>This profile defines a representation of information of the requested service including the requesting practitioner as part of Medicare Benefits Schedule (MBS) claim item records.</td>
       </tr>
 </tbody>
</table>
<br/>

###  Pharmaceutical Benefits Schedule (PBS) claim item record

Profiles that define representation of Pharmaceutical Benefits Schedule (PBS) claim items:

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
         <td>This profile defines a representation of prescription data to as part of a PBS claim item.</td>
      </tr>
      <tr>
         <td><a href="StructureDefinition-medication-pbs.html">Medication Pharmaceutical Benefits Scheme</a></td>
         <td>This profile defines a representation of pharmaceutical item data as part of a PBS claim item.</td>
      </tr>
 </tbody>
</table>
<br/>


