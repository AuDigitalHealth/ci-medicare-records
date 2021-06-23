#### Australian Immunisation Register Notice *[[Active](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

This profile defines a representation of an Australian Immunisation Register (AIR) notice for an individual. A notice may include information that an individual has an exemption record or has finished a National Immunisation Program schedule.

##### **Usage scenarios**
The following are the usage scenarios expected:
* An individual’s Australian Immunisation Register records are uploaded to the My Health Record system from a Medicare Repository

##### **Each Flag SHALL have**
1. a profile assertion to this profile
1. an identifier for this notice
1. a status of this notice set to active
1. a category to indicate this is an AIR notice
1. a code that includes the notice text
1. a patient

##### **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
   * category
   * code
 * The system SHALL be able to take the following elements into account when performing processing:
    * identifier
    * patient
    
##### **Profile-specific implementation guidance**
* The notice text is sent in the text portion of code