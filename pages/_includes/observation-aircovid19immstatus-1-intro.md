#### Australian Immunisation Register COVID-19 Immunisation Status *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

#### **Usage scenarios**
The following are the expected usage scenarios this profile is intended to support:
* Medicare sends Australian Immunisation Register records to the My Health Record system

##### **Each Observation SHALL have**
1.	a profile assertion to this profile 
2.	an identifier
3.	a code that indicates this is AIR COVID-19 immunisation status
4.	a patient
5.	an immunisation status

#####  **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
    * code
    * valueCodeableConcept
    * comment
* The system SHALL be able to take the following elements into account when performing processing:
    * identifier
    * subject

##### **Profile-specific implementation guidance**
* If the immunisation status value is text, it is sent in the text portion of valueCodeableConcept

