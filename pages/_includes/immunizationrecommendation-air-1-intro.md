#### Australian Immunisation Register Immunisation Recommendation  *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

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
* in order to provide identification of a target disease to be protected against and the due date, the resource requires a forecast status; this data is not available so forecastStatus has been set to NAVU Not Available

