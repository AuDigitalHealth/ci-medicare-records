# {{ page.title }}
The following extensions are defined as part of this implementation guide.

<table class="list" width="100%">
    <tr>
        <th>Extension</th>
        <th>Usage scenario</th>
        <th>Type</th>
        <th>Context</th>
        <th>Profile context</th>
    </tr>
    <tr>
        <td><a href="StructureDefinition-extension-donationdecision.html">Consent Donation Decision</a></td>
        <td>Australian Organ Donor Register record</td>
        <td><a href="http://hl7.org/fhir/STU3/datatypes.html#CodeableConcept">CodeableConcept</a></td>
        <td><a href="http://hl7.org/fhir/STU3/Consent.html">Consent</a></td>
        <td><a href="StructureDefinition-consent-aodr.html">Consent Australian Organ Donor Register</a></td>
    </tr>
    <tr>
        <td><a href="StructureDefinition-extension-dateinitialregistration.html">Date Initial Registration</a></td>
        <td>Australian Organ Donor Register record</td>
        <td><a href="http://hl7.org/fhir/STU3/datatypes.html#dateTime">dateTime</a></td>
        <td><a href="http://hl7.org/fhir/STU3/Resource.html">Resource</a></td>
        <td><a href="StructureDefinition-consent-aodr.html">Consent Australian Organ Donor Register</a></td>
    </tr>
    <tr>
        <td><a href="StructureDefinition-vaccine-serial-number-1.html">Vaccine Vial Serial Number</a></td>
        <td>Australian Immunisation Register record</td>
        <td><a href="http://hl7.org/fhir/STU3/datatypes.html#string">string</a></td>
        <td><a href="http://hl7.org/fhir/STU3/immunization-definitions.html#Immunization">Immunization</a></td>
        <td><a href="StructureDefinition-immunization-air.html">Australian Immunisation Register Immunisation</a></td>
    </tr>
</table>