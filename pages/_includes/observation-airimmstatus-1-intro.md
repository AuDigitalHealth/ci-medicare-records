#### Australian Immunisation Register Immunisation Status *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

#### Usage Scenarios
The following are the overarching usage scenarios this profile is intended to support:
* Services Australia Medicare sends records of immunisation status the My Health Record system

#### Implementation guidance
For the overarching usage scenarios in this implementation guide it is expected that:
* if the immunisation status is 'up to date' code 171258008 \|Up-to-date with vaccinations\| will be sent in Observation.value
* if the immunisation status is 'not up to date' code 171259000 \|Not up to date with vaccinations\| will be sent in Observation.value