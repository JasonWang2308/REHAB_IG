# MedicationAdministrationIdentifier - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationAdministrationIdentifier**

## SearchParameter: MedicationAdministrationIdentifier 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/MedicationAdministration-identifier | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:MedicationAdministrationIdentifier |

 
Return administrations with this external identifier 

## MedicationAdministrationIdentifier

Parameter `identifier`:`token`

Return administrations with this external identifier

| | |
| :--- | :--- |
| Resource | [MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) |
| Expression | `MedicationAdministration.​identifier` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "MedicationAdministrationIdentifier",
  "url" : "http://example.org/fhir/SearchParameter/MedicationAdministration-identifier",
  "version" : "0.1.0",
  "name" : "MedicationAdministrationIdentifier",
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
  "description" : "Return administrations with this external identifier",
  "code" : "identifier",
  "base" : ["MedicationAdministration"],
  "type" : "token",
  "expression" : "MedicationAdministration.​identifier"
}

```
