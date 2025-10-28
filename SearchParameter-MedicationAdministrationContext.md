# MedicationAdministrationContext - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationAdministrationContext**

## SearchParameter: MedicationAdministrationContext 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/MedicationAdministration-context | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:MedicationAdministrationContext |

 
Return administrations that share this encounter or episode of care 

## MedicationAdministrationContext

Parameter `context`:`reference`

Return administrations that share this encounter or episode of care

| | |
| :--- | :--- |
| Resource | [MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) |
| Expression | `MedicationAdministration.​context` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "MedicationAdministrationContext",
  "url" : "http://example.org/fhir/SearchParameter/MedicationAdministration-context",
  "version" : "0.1.0",
  "name" : "MedicationAdministrationContext",
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
  "description" : "Return administrations that share this encounter or episode of care",
  "code" : "context",
  "base" : ["MedicationAdministration"],
  "type" : "reference",
  "expression" : "MedicationAdministration.​context"
}

```
