# {{ page.title }}
{:.no_toc}
<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
* Do not remove this line (it will not be displayed)
{:toc}


### Version = 2.0.1
- Publication date: **IN PROGRESS**
- Publication status: **PROGRESSING THROUGH ASSURANCE**
- url: <https://build.fhir.org/ig/AuDigitalHealth/ci-medicare-records/branches/2.1.0/>
- Based on FHIR version : 3.0.2

This version is developed for the Enhanced Use of Immunisation Records project. This version addresses the changes in scope to the FHIR payload in this project.

**Changes in this version**

Amended:

- Australian Immunisation Register Immunisation - removed constraints on population of Immunization.patient.identifier
- Australian Immunisation Register Notice - removed constraints on population of Flag.subject.identifier
- Consent Australian Organ Donor Register - corrected category slicing [ci-medicare-records #6](https://github.com/AuDigitalHealth/ci-medicare-records/issues/6), corrected FHIRPath for inv-dh-cons-01 & inv-dh-cons-02 [ci-medicare-records #5](https://github.com/AuDigitalHealth/ci-medicare-records/issues/5), corrected Consent.except.action to patternCodeableConcept [ci-medicare-records #2](https://github.com/AuDigitalHealth/ci-medicare-records/issues/2)
- Explanation of Benefit Medicare - corrected FHIRPath for inv-dh-eob-01, inv-dh-eob-02 & inv-dh-eob-04[ci-medicare-records #4](https://github.com/AuDigitalHealth/ci-medicare-records/issues/4)

Removed:
- profile Australian Immunisation Register Immunisation Status
- profile Australian Immunisation Register COVID-19 Immunisation Status
- profile Australian Immunisation Register Immunisation Recommendation
- profile Declared Disclaimer
- extension Immunisation Dose Schedule

<br/><br/>
### Version = 2.0.0
- Publication date: 27 Novemeber 2020
- Publication status: Draft for external use [THIS STATUS WAS ISSUED IN ERROR AND IS WITHDRAWN]
- url: N/A
- Based on FHIR version : 3.0.2
- Archived release location: <https://github.com/AuDigitalHealth/ci-medicare-records/releases/tag/MR-2.0.0-2020NOV>

Pre-release for review. This version is developed for the Enhanced Use of Immunisation Records project.

**Changes in this version**

Added:
- profile Australian Immunisation Register Immunisation Status
- profile Australian Immunisation Register COVID-19 Immunisation Status
- profile Australian Immunisation Register Notice
- profile Australian Immunisation Register Immunisation Recommendation
- profile Declared Disclaimer
- extension Immunisation Dose Schedule
- extension Vaccine Serial Number

Amended:
- profile Australian Immunisation Register Immunisation - corrected to represent only administered vaccines, added vaccine serial number and schedule information

Removed: 
- extension Immunisation Cancellation Period
                  
<br/><br/>          
### Version = 1.0.0
- Publication date: 1 November 2018
- Publication status: Approved for external use
- url: <https://developer.digitalhealth.gov.au/sites/default/files/specifications/clinical-documents/ep-2746-2018/dh-2738-2018/index.html>
- Based on FHIR version : 3.0.1
  - Archived release location: TBD 

The Medicare Records FHIR Implementation Guide was developed in support of the Medicare Document Simplification work package for My Health Record system release v9.3.