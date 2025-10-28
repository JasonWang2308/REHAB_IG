# MedicationAdministrationReasongiven - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationAdministrationReasongiven**

## SearchParameter: MedicationAdministrationReasongiven 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/MedicationAdministration-reason-given | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:MedicationAdministrationReasongiven |

 
Reasons for administering the medication 

## MedicationAdministrationReasongiven

Parameter `reason-given`:`token`

Reasons for administering the medication

| | |
| :--- | :--- |
| Resource | [MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) |
| Expression | `MedicationAdministration.​reasonCode` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "MedicationAdministrationReasongiven",
  "url" : "http://example.org/fhir/SearchParameter/MedicationAdministration-reason-given",
  "version" : "0.1.0",
  "name" : "MedicationAdministrationReasongiven",
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
  "description" : "Reasons for administering the medication",
  "code" : "reason-given",
  "base" : ["MedicationAdministration"],
  "type" : "token",
  "expression" : "MedicationAdministration.​reasonCode"
}

```
