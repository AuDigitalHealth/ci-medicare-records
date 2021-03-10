The purpose of this profile is to describe a declared disclaimer included with some information.

##### **Usage scenarios**
The following are the usage scenarios expected:
* Medicare sends Australian Immunisation Register records to the My Health Record system

##### **Each Basic SHALL have**
1. a profile assertion to this profile
2. a disclaimer text
3. an identifier
1. a code indicating this is an AIR explanatory note

#####  **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
    * text
    * code
* The system SHALL be able to take the following elements into account when performing processing:
    * identifier

##### **Profile-specific implementation guidance**
* AIR explanatory text is sent in text

