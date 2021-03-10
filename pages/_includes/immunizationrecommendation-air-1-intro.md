The purpose of this profile is to define a representation of the antigen(s) for which an individual is due within the National Immunisation Program, based upon their history of immunisations.

##### **Usage scenarios**
The following are the usage scenarios expected:
* Medicare sends Australian Immunisation Register records to the My Health Record system

##### **Each ImmunizationRecommendation SHALL have**
1. a profile assertion to this profile
1. an identifier for this next immunisation due record
1. a patient
1. a creation date of this record
1. an antigen that is due next  
1. a forecast status set to NAVU Not Available
1. a due date


##### **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
    * recommendation
    * recommendation.date
    * recommendation.targetDisease
    * recommendation.dateCriterion
    * recommendation.dateCriterion.value    
* The system SHALL be able to take the following elements into account when performing processing:
    * identifier
    * patient

##### **Profile-specific implementation guidance**
* The patient is identified with an IHI in patient.identifier, not with a reference to a Patient resource