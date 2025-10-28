# MedicationAdministrationEffectivetime - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationAdministrationEffectivetime**

## SearchParameter: MedicationAdministrationEffectivetime 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/MedicationAdministration-effective-time | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:MedicationAdministrationEffectivetime |

 
Date administration happened (or did not happen) 

## MedicationAdministrationEffectivetime

Parameter `effective-time`:`date`

Date administration happened (or did not happen)

| | |
| :--- | :--- |
| Resource | [MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) |
| Expression | `MedicationAdministration.​effective` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "MedicationAdministrationEffectivetime",
  "url" : "http://example.org/fhir/SearchParameter/MedicationAdministration-effective-time",
  "version" : "0.1.0",
  "name" : "MedicationAdministrationEffectivetime",
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
  "description" : "Date administration happened (or did not happen)",
  "code" : "effective-time",
  "base" : ["MedicationAdministration"],
  "type" : "date",
  "expression" : "MedicationAdministration.​effective"
}

```
