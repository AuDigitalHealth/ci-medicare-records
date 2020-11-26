#### Australian Immunisation Register COVID-19 Immunisation Status *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

#### Usage Scenarios
The following are the expected usage scenarios this profile is intended to support:
* Services Australia Medicare sends Australian Immunisation Register records to the My Health Record system

#### Implementation guidance
For the overarching usage scenarios in this implementation guide it is expected that:
* the patient is identified with an IHI in subject.identifier, not with a reference to a Patient resource
* if the immunisation status value is text, it is sent in the text portion of valueCodeableConcept