# MedicationAdministrationRequest - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationAdministrationRequest**

## SearchParameter: MedicationAdministrationRequest 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/MedicationAdministration-request | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:MedicationAdministrationRequest |

 
The identity of a request to list administrations from 

## MedicationAdministrationRequest

Parameter `request`:`reference`

The identity of a request to list administrations from

| | |
| :--- | :--- |
| Resource | [MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) |
| Expression | `MedicationAdministration.​request` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "MedicationAdministrationRequest",
  "url" : "http://example.org/fhir/SearchParameter/MedicationAdministration-request",
  "version" : "0.1.0",
  "name" : "MedicationAdministrationRequest",
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
  "description" : "The identity of a request to list administrations from",
  "code" : "request",
  "base" : ["MedicationAdministration"],
  "type" : "reference",
  "expression" : "MedicationAdministration.​request"
}

```
