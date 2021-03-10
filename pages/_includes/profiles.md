# {{ page.title }}
The [profiles](http://hl7.org/fhir/STU3/profiling.html) listed below are defined as part of this implementation guide. HL7 Australia base profiles referenced by this implementation guide can be found in [Australian Base Implementation Guide [HL7AUF3B2]](index.html#HL7FHIR3).

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
     <td><a href="StructureDefinition-observation-airimmstatus-1.html">Australian Immunisation Register Immunisation Status</a></td>
     <td>The purpose of this profile is to describe the immunisation status for an individual specific to the National Immunisation Program childhood and adolescent vaccination schedules, and if the individual is on a catch up schedule.</td>
  </tr>
  <tr>
     <td><a href="StructureDefinition-observation-aircovid19immstatus-1.html">Australian Immunisation Register COVID-19 Immunisation Status</a></td>
     <td>The purpose of this profile is to describe the Australian Immunisation Register (AIR) COVID-19 immunisation status for an individual.</td>
  </tr>

  <tr>
     <td><a href="StructureDefinition-immunizationrecommendation-air-1.html">Australian Immunisation Register Immunisation Recommendation</a></td>
     <td>The purpose of this profile is to define a representation of the antigen(s) for which an individual is due within the National Immunisation Program, based upon their history of immunisations.</td>
   </tr>
   <tr>
      <td><a href="StructureDefinition-flag-air-1.html">Australian Immunisation Register Notice</a></td>
      <td>The purpose of this profile is to define a representation of the Australian Immunisation Register (AIR) notice such as notice an individual has an exemption record or has finished a National Immunisation Program schedule.</td>
   </tr>
   <tr>
      <td><a href="StructureDefinition-basic-decldiscl-1.html">Declared Disclaimer</a></td>
      <td>The purpose of this profile is to describe a declared disclaimer included with some information.</td>
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




