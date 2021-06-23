#### Australian Immunisation Register Immunisation *[[Active](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

This profiles defines a representation of the record of an administered vaccination, for an individual, held in the Australian Immunisation Register (AIR).

##### **Usage scenarios**
The following are the usage scenarios expected:
* An individual’s Australian Immunisation Register records are uploaded to the My Health Record system from a Medicare Repository

##### **Each Immunization SHALL have**
1. a profile assertion to this profile
1. an identifier for this immunisation record
1. a status of the vaccination event set to completed
1. a flag to indicate that the vaccine was administered
1. a vaccine
1. a patient
1. a date that the vaccine was administered 
1. a flag to indicate this data is based on information from the person who administered the vaccine
1. an antigen administered according to the vaccine administered
1. a dose status data set to NAVU Not Available 

##### **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
   * vaccine-serial-number-1
   * status
   * notGiven
   * vaccineCode
   * date
   * primarySource
   * lotNumber
   * vaccinationProtocol
   * vaccinationProtocol.doseSequence
   * vaccinationProtocol.targetDisease
* The system SHALL be able to take the following elements into account when performing processing:
    * identifier
    * patient

##### **Profile-specific implementation guidance**
No specific guidance.

