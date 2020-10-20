#### Base Organization *[[Active](http://hl7.org/fhir/stu3/valueset-publication-status.html)]*

#### Implementation guidance

For the overarching usage scenarios in this implementation guide it is recommended that:
* an Australian address conforms to [AU Base Address](https://hl7.org.au/fhir/base/aubase1.1/StructureDefinition-au-address.html)
* if more than one identifier is sent, only one of each type is sent
* if a resource is referenced rather than identified in the applicable element, the referenced resource should be [contained](https://www.hl7.org/fhir/STU3/references.html#contained)

This profile is referenced by  [Patient with Mandatory IHI](StructureDefinition-patient-ihi-1.html) and TBD.
