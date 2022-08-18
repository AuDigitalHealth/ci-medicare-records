# {{ page.title }}
{:.no_toc}
<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
* Do not remove this line (it will not be displayed)
{:toc}


### Version = 2.2.0
- Publication date: **IN PROGRESS**
- Publication status: **PROGRESSING THROUGH ASSURANCE**
- url: <http://ns.electronichealth.net.au/fhir/ImplementationGuide/au.digitalhealth.stu3.medicare-records/2.2.0>
- Based on FHIR version : 3.0.2

This version is developed for the HDR Upgrade project. This version clarifies the scope of the live feed FHIR payload to the MHR system.

**Changes in this version**

Amended:

- ADHA Australian Organ Donor Register Consent - remove support for extension Date of Initial Registration [ci-medicare-records #23](https://github.com/AuDigitalHealth/ci-medicare-records/issues/23)
- ADHA Medicare ExplanationOfBenefit - remove support for ExplanationOfBenefit.referral [ci-medicare-records #21](https://github.com/AuDigitalHealth/ci-medicare-records/issues/21)
- extension Consent Donation Decision - refactored to remove erroneous slicing [ci-medicare-records #20](https://github.com/AuDigitalHealth/ci-medicare-records/issues/20), correct description [ci-medicare-records #22](https://github.com/AuDigitalHealth/ci-medicare-records/issues/22) 
- extension Vaccine Vial Serial Number - refactored to remove erroneous slicing [ci-medicare-records #18](https://github.com/AuDigitalHealth/ci-medicare-records/issues/18)
- added profile-specific implementation guidance to the page for ADHA Medicare ExplanationOfBenefit to include practitioner-classification extension [ci-medicare-records #24](https://github.com/AuDigitalHealth/ci-medicare-records/issues/24)

Removed:
- profile ADHA MBS DVA ReferralRequest [ci-medicare-records #21](https://github.com/AuDigitalHealth/ci-medicare-records/issues/21)
- extension Date of Initial Registration [ci-medicare-records #23](https://github.com/AuDigitalHealth/ci-medicare-records/issues/23)

---

### Version = 2.1.0
- Publication date: **IN PROGRESS**
- Publication status: **PROGRESSING THROUGH ASSURANCE**
- url: <http://ns.electronichealth.net.au/fhir/ImplementationGuide/au.digitalhealth.stu3.medicare-records/2.1.0>
- Based on FHIR version : 3.0.2

This version is developed for the Enhanced Use of Immunisation Records project. This version addresses the changes in scope to the FHIR payload in this project.

**Changes in this version**

Amended:

- ADHA Australian Immunisation Register Immunization - removed constraints on population of Immunization.patient.identifier [ci-medicare-records #15](https://github.com/AuDigitalHealth/ci-medicare-records/issues/15)
- ADHA Australian Immunisation Register Flag - removed constraints on population of Flag.subject.identifier [ci-medicare-records #15](https://github.com/AuDigitalHealth/ci-medicare-records/issues/15)
- ADHA Australian Organ Donor Register Consent - technical correction to category slicing [ci-medicare-records #6](https://github.com/AuDigitalHealth/ci-medicare-records/issues/6), corrected FHIRPath for inv-dh-cons-01 & inv-dh-cons-02 [ci-medicare-records #5](https://github.com/AuDigitalHealth/ci-medicare-records/issues/5), corrected Consent.except.action to patternCodeableConcept [ci-medicare-records #2](https://github.com/AuDigitalHealth/ci-medicare-records/issues/2)
- ADHA Medicare ExplanationOfBenefit - technical correction to FHIRPath for inv-dh-eob-01, inv-dh-eob-02 & inv-dh-eob-04 [ci-medicare-records #4](https://github.com/AuDigitalHealth/ci-medicare-records/issues/4)
- technical correction to revert HL7 AU Base implementation guide dependency version to v0.9.3 12 September 2018 [ci-medicare-records #15](https://github.com/AuDigitalHealth/ci-medicare-records/issues/15)
- applied 2022 naming policy to title and name of structures [ci-medicare-records #17](https://github.com/AuDigitalHealth/ci-medicare-records/issues/17)

Removed:
- profile Australian Immunisation Register Immunisation Status [ci-medicare-records #16](https://github.com/AuDigitalHealth/ci-medicare-records/issues/16)
- profile Australian Immunisation Register COVID-19 Immunisation Status [ci-medicare-records #16](https://github.com/AuDigitalHealth/ci-medicare-records/issues/16)
- profile Australian Immunisation Register Immunisation Recommendation [ci-medicare-records #16](https://github.com/AuDigitalHealth/ci-medicare-records/issues/16)
- profile Declared Disclaimer [ci-medicare-records #16](https://github.com/AuDigitalHealth/ci-medicare-records/issues/16)
- extension Immunisation Dose Schedule [ci-medicare-records #16](https://github.com/AuDigitalHealth/ci-medicare-records/issues/16)

---

### Version = 2.0.0
- Publication date: 27 November 2020
- Publication status: Draft for external use [THIS STATUS WAS ISSUED IN ERROR AND IS CORRECTED TO: Draft for external review]
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

---

### Version = 1.0.0
- Publication date: 1 November 2018
- Publication status: Approved for external use
- url: <http://ns.electronichealth.net.au/fhir/ImplementationGuide/au.digitalhealth.stu3.medicare-records/1.0.0>
- Based on FHIR version : 3.0.1 

The Australian Digital Health Agency Medicare Records FHIR Implementation Guide was developed in support of the Medicare Document Simplification work package for My Health Record system release v9.3.

---