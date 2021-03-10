#### Australian Immunisation Register Immunisation Status *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

#### Usage scenarios
The following are the expected usage scenarios this profile is intended to support:
* Medicare sends Australian Immunisation Register records to the My Health Record system

#### Implementation guidance
For the overarching usage scenarios in this implementation guide it is expected that:
* the patient is identified with an IHI in subject.identifier, not with a reference to a Patient resource
* if the immunisation status is 'up to date', code 171258008 \|Up-to-date with vaccinations\| is sent in valueCodeableConcept
* if the immunisation status is 'not up to date', code 171259000 \|Not up to date with vaccinations\| is sent in valueCodeableConcept