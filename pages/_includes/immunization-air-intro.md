#### Immunization Australian Immunisation Register  *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*
The purpose of this profile is to define a representation of vaccination information from the Australian Immunisation Register.

#### Usage Scenarios
The following are the overarching usage scenarios this profile is intended to support:
* DHS Medicare sends records of administered vaccines to the My Health Record system

#### Implementation guidance
For the overarching usage scenarios in this implementation guide it is expected that:
* if a resource is referenced rather than identified in the applicable element, the referenced resource should be [contained](https://www.hl7.org/fhir/STU3/references.html#contained)
* in order to provide identification of a target disease to be protected against, the resource requires a dose status; this data is not available so doseStatus has been set to NAVU Not Available

