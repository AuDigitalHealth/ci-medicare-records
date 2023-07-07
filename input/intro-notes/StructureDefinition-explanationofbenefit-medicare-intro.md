### Usage scenarios
The following are the usage scenarios expected:
* An individual’s MBS claim item records are uploaded to the My Health Record system from a Medicare repository
* An individual’s PBS claim item records are uploaded to the My Health Record system from a Medicare repository


### Each Explanation of Benefit SHALL have
1. a profile assertion to this profile
1. an identifier for this explanation of benefit record 
1. a patient
1. a creation date
1. an identification of the Medicare benefit (subtype or item.category)
1. an item that was claimed
1. a date of supply or service


### Must Support
In the context of this profile [Must Support](http://hl7.org/fhir/STU3/conformance-rules.html#mustSupport) SHALL be interpreted as follows.
* The system SHALL be able to store and retrieve the following elements:
    * status
    * type
    * subtype
    * created
    * provider
    * prescription
    * item
    * item.sequence
    * item.category
    * item.service
    * item.serviced
    * item.quantity
* The system SHALL be able to take the following elements into account when performing processing:
    * identifier
    * patient
 
 
### Profile-specific implementation guidance
* The patient resource should be identified in the patient element with a [logical reference](https://www.hl7.org/fhir/STU3/references.html#logical), i.e. an Australian IHI
* PBS record: 
    * An ExplanationOfBenefit for a PBS record will represent prescription data as a MedicationRequest, including date of prescribing, number of repeats, and quantity
    * Generic name of a PBS item can be represented by the supplied item service code
    * Date of supply of the item is represented by item.serviced[x]
* MBS record: 
    * Whether a service was provided in a hospital is indicated by the use and value of item.location
    * Date of service is represented by item.serviced[x]
    * Provider role is represented in a contained Practitioner resource using the [practitioner-classification](http://hl7.org/fhir/STU3/extension-practitioner-classification.html) extension 




