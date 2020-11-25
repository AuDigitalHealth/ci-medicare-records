#### Australian Immunisation Register Immunisation Status *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

#### Usage Scenarios
The following are the expected usage scenarios this profile is intended to support:
* Services Australia Medicare sends immunisation information about a patient to the My Health Record

#### Implementation guidance
For the overarching usage scenarios in this implementation guide it is expected that:
* the patient is identified with an IHI in subject.identifier, not with a reference to a Patient resource
* resources in an immunisation summary share a common value in identifier
* if the immunisation status is 'up to date', code 171258008 \|Up-to-date with vaccinations\| is sent in valueCodeableConcept
* if the immunisation status is 'not up to date', code 171259000 \|Not up to date with vaccinations\| is sent in valueCodeableConcept