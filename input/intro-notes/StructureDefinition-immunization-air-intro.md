The purpose of this profile is to define a representation of an administered vaccination, for an individual, held in the Australian Immunisation Register (AIR) for the electronic exchange of digital health information between Medicare repositories and the My Health Record system infrastructure in Australia.


### Usage scenarios
The following are the usage scenarios expected:
* An individual’s Australian Immunisation Register record is uploaded to the My Health Record system from a Medicare repository


### Each Immunization SHALL have
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


### Must Support
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
   * serialNumber
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


### Profile-specific implementation guidance
* The patient resource should be identified in the patient element with a [logical reference](https://www.hl7.org/fhir/STU3/references.html#logical), i.e. an Australian IHI


