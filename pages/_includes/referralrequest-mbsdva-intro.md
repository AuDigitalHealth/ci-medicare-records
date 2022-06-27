#### Referral Request Medicare Benefits Schedule Department of Veterans’ Affairs *[[Active](http://hl7.org/fhir/STU3/valueset-publication-status.html)]*

The purpose of this profile is to define a representation of service item claimed information, including practitioner that requested the service, in a claim against the Medicare Benefits Schedule (MBS) or Department of Veterans' Affairs (DVA) for the electronic exchange of digital health information between Medicare repositories and the My Health Record system infrastructure in Australia.


##### **Usage scenarios**
The following are the usage scenarios expected:
* An individual’s Medicare Benefits Schedule (MBS) claim item records are uploaded to the My Health Record system from a Medicare repository


##### **Each ReferralRequest SHALL have**
1. a profile assertion to this profile 
1. a status of referral request
1. an intent
1. a patient
1. a practitioner that requested the service


##### **Must Support**
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
    * status
    * intent
    * requester
    * requester.agent
    * requester.onBehalfOf
    * specialty
* The system SHALL be able to take the following elements into account when performing processing:
   * identifier
    * subject


##### **Profile-specific implementation guidance**
* The patient resource should be identified in the subject element with a [logical reference](https://www.hl7.org/fhir/STU3/references.html#logical), i.e. an Australian IHI
