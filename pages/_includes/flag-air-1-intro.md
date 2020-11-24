#### Australian Immunisation Register Notice  *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

#### Usage Scenarios
The following are the expected usage scenarios this profile is intended to support:
* Services Australia Medicare sends to the My Health Record system an Australian Immunisation Register (AIR) bundle with
  * one or more records of administered vaccines
  * zero or one records of immunisation status
  * zero of one records of COVID-19 immunisation status
  * zero or more records of vaccinations not received and due in the next schedule point
  * zero of more notices 
  * one explanatory text

#### Implementation guidance
For the overarching usage scenarios in this implementation guide it is expected that:
* the patient is identified with an IHI in subject.identifier, not with a reference to a Patient resource
* notice text is sent in the text portion of code

