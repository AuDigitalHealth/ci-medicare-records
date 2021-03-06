#### Medication Pharmaceutical Benefits Scheme *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

This profile defines a representation of medication data to support representation of PBS claim items.

##### **Usage scenarios**
The following are the usage scenarios expected:
* Medicare sends PBS records to the My Health Record system

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
