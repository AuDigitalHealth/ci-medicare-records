#### Australian Immunisation Register Notice  *[[Draft](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

#### Usage scenarios
The following are the usage scenarios expected:
* Medicare sends Australian Immunisation Register records to the My Health Record system

#### **Each Flag SHALL have**
1. a profile assertion to this profile
1. an identifier for this notice
1. a status of this notice
1. a category to indicate this is an AIR notice
1. a code that includes the notice text
1. a patient

#####  **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
   * category
   * code
 * The system SHALL be able to take the following elements into account when performing processing:
    * identifier
    * patient
    
#### **Profile-specific implementation guidance**
No specific guidance.