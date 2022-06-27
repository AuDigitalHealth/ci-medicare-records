#### Medication Pharmaceutical Benefits Scheme *[[Active](http://hl7.org/fhir/STU3/valueset-publication-status.html)]*

The purpose of this profile is to define a representation of medicinal product information for a prescription item claimed in a claim against the Pharmaceutical Benefits Schedule (PBS) or Repatriation Pharmaceutical Benefits Scheme (RPBS) for the electronic exchange of health information between Medicare repositories and the My Health Record system infrastructure in Australia.


##### **Usage scenarios**
The following are the usage scenarios expected:
* An individual’s Pharmaceutical Benefits Schedule (PBS) records are uploaded to the My Health Record system from a Medicare repository


##### **Each Medication SHALL have**
1. a code identifying the medication


##### **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
    * code
* The system SHALL be able to take the following elements into account when performing processing:
    * manufacturer


##### **Profile-specific implementation guidance**
No specific guidance.
