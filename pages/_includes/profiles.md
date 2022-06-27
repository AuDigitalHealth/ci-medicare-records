# {{ page.title }}
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
     <td><a href="StructureDefinition-immunization-air.html">Australian Immunisation Register Immunisation</a></td>
     <td>This profile defines a representation of the record of an administered vaccination, for an individual, held in the Australian Immunisation Register.</td>
  </tr>
   <tr>
      <td><a href="StructureDefinition-flag-air-1.html">Australian Immunisation Register Notice</a></td>
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
       <td><a href="StructureDefinition-consent-aodr.html">Consent Australian Organ Donor Register</a></td>
       <td>This profile defines a representation of donation decision information from the Australian Organ Donor Register.</td>
     </tr>
     <tr>
       <td><a href="StructureDefinition-bodysite-aodr.html">BodySite Australian Organ Donor Register</a></td>
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
         <td><a href="StructureDefinition-explanationofbenefit-medicare.html">Explanation of Benefit Medicare</a></td>
         <td>This profile defines a representation of PBS claim items or MBS claim items.</td>
      </tr>
      <tr>
         <td><a href="StructureDefinition-referralrequest-mbsdva.html">Referral Request Medicare Benefits Schedule Department of Veterans’ Affairs</a></td>
         <td>This profile defines a representation of information of the requested service including the requesting practitioner as part of MBS claim item records.</td>
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
         <td><a href="StructureDefinition-explanationofbenefit-medicare.html">Explanation of Benefit Medicare</a></td>
         <td>This profile defines a representation of PBS claim items or MBS claim items.</td>
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


