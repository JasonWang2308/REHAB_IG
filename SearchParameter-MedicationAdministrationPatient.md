# MedicationAdministrationPatient - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationAdministrationPatient**

## SearchParameter: MedicationAdministrationPatient 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/MedicationAdministration-patient | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:MedicationAdministrationPatient |

 
The identity of a patient to list administrations for 

## MedicationAdministrationPatient

Parameter `patient`:`reference`

The identity of a patient to list administrations for

| | |
| :--- | :--- |
| Resource | [MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) |
| Expression | `MedicationAdministration.​subject.​where(resolve() is Patient)` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "MedicationAdministrationPatient",
  "url" : "http://example.org/fhir/SearchParameter/MedicationAdministration-patient",
  "version" : "0.1.0",
  "name" : "MedicationAdministrationPatient",
  "status" : "active",
  "date" : "2025-10-28T11:34:57+08:00",
  "publisher" : "Example Publisher",
  "contact" : [
    {
      "name" : "Example Publisher",
      "telecom" : [
        {
          "system" : "url",
          "value" : "http://example.org/example-publisher"
        }
      ]
    }
  ],
  "description" : "The identity of a patient to list administrations for",
  "code" : "patient",
  "base" : ["MedicationAdministration"],
  "type" : "reference",
  "expression" : "MedicationAdministration.​subject.​where(resolve() is Patient)"
}

```
