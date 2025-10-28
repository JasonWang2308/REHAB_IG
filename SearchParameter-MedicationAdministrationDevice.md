# MedicationAdministrationDevice - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationAdministrationDevice**

## SearchParameter: MedicationAdministrationDevice 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/MedicationAdministration-device | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:MedicationAdministrationDevice |

 
Return administrations with this administration device identity 

## MedicationAdministrationDevice

Parameter `device`:`reference`

Return administrations with this administration device identity

| | |
| :--- | :--- |
| Resource | [MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) |
| Expression | `MedicationAdministration.​device` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "MedicationAdministrationDevice",
  "url" : "http://example.org/fhir/SearchParameter/MedicationAdministration-device",
  "version" : "0.1.0",
  "name" : "MedicationAdministrationDevice",
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
  "description" : "Return administrations with this administration device identity",
  "code" : "device",
  "base" : ["MedicationAdministration"],
  "type" : "reference",
  "expression" : "MedicationAdministration.​device"
}

```
