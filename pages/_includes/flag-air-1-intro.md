#### Australian Immunisation Register Notice *[[Active](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

The purpose of this profile is to define a notice, such as an exemption record or notification of completion of an immunisation schedule, from the Australian Immunisation Register for the electronic exchange of digital health information between Medicare repositories and the My Health Record system infrastructure in Australia.


##### **Usage scenarios**
The following are the usage scenarios expected:
* An individual’s Australian Immunisation Register records are uploaded to the My Health Record system from a Medicare repository


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
* The patient resource should be identified in the subject element with a [logical reference](https://www.hl7.org/fhir/STU3/references.html#logical), i.e. an Australian IHI
* The notice text is sent in the text portion of code