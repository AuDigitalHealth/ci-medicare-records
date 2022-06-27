#### BodySite Australian Organ Donor Register *[[Active](http://hl7.org/fhir/STU3/valueset-publication-status.html)]*

The purpose of this profile is to represent an organ or tissue that may be donated in the event of an individual's death for the electronic exchange of organ donation as recorded on the Australian Organ Donor Register between Medicare repositories and the My Health Record system infrastructure in Australia.


##### **Usage scenarios**
The following are the usage scenarios expected:
* An individual’s Australian Organ Donor Register (AODR) record is uploaded to the My Health Record system from a Medicare repository


##### **Each BodySite SHALL have**
1. a code identifying the organ or tissue
1. a patient


##### **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
    * code
* The system SHALL be able to take the following elements into account when performing processing:
    * patient


##### **Profile-specific implementation guidance**
* The patient resource should be identified in the patient element with a [logical reference](https://www.hl7.org/fhir/STU3/references.html#logical), i.e. an Australian IHI

