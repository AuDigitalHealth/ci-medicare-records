### Usage scenarios
The following are the usage scenarios expected:
* An individual’s Australian Organ Donor Register record is uploaded to the My Health Record system from a Medicare repository


### Each BodySite SHALL have
1. a code identifying the organ or tissue
1. a patient


### Must Support
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
    * code
* The system SHALL be able to take the following elements into account when performing processing:
    * patient


### Profile-specific implementation guidance
* The patient resource should be identified in the patient element with a [logical reference](https://www.hl7.org/fhir/STU3/references.html#logical), i.e. an Australian IHI

