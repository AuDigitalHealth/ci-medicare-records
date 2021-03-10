The purpose of this profile is to describe the immunisation status for an individual specific to the National Immunisation Program childhood and adolescent vaccination schedules, and if the individual is on a catch up schedule.

##### **Usage scenarios**
The following are the usage scenarios expected:
* Medicare sends Australian Immunisation Register records to the My Health Record system

##### **Each Observation SHALL have**
1.	a profile assertion to this profile 
2.	an identifier
3.	a code that indicates this is AIR immunisation status
4.	a patient
5.	an immunisation status

#####  **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
    * code
    * value[x]
    * comment
* The system SHALL be able to take the following elements into account when performing processing:
    * identifier
    * subject

##### **Profile-specific implementation guidance**
* The patient is identified with an IHI in subject.identifier, not with a reference to a Patient resource
* If the immunisation status is 'up to date', code 171258008 \|Up-to-date with vaccinations\| is sent in valueCodeableConcept
* If the immunisation status is 'not up to date', code 171259000 \|Not up to date with vaccinations\| is sent in valueCodeableConcept
