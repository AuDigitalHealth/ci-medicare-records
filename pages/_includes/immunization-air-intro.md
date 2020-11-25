#### Australian Immunisation Register Immunisation  *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

#### Usage Scenarios
The following are the expected usage scenarios this profile is intended to support:
* Services Australia Medicare sends immunisation information about a patient to the My Health Record

#### Implementation guidance
For the overarching usage scenarios in this implementation guide it is expected that:
* the patient is identified with an IHI in patient.identifier, not with a reference to a Patient resource
* resources in an immunisation summary share a common value in identifier
* in order to provide identification of a target disease to be protected against, the resource requires a dose status; this data is not available so vaccinationProtocol.doseStatus is set to NAVU Not Available
* the antigen is recorded as text in vaccinationProtocol.targetDisease