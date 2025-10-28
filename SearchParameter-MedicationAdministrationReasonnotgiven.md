# MedicationAdministrationReasonnotgiven - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationAdministrationReasonnotgiven**

## SearchParameter: MedicationAdministrationReasonnotgiven 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/MedicationAdministration-reason-not-given | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:MedicationAdministrationReasonnotgiven |

 
Reasons for not administering the medication 

## MedicationAdministrationReasonnotgiven

Parameter `reason-not-given`:`token`

Reasons for not administering the medication

| | |
| :--- | :--- |
| Resource | [MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) |
| Expression | `MedicationAdministration.​statusReason` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "MedicationAdministrationReasonnotgiven",
  "url" : "http://example.org/fhir/SearchParameter/MedicationAdministration-reason-not-given",
  "version" : "0.1.0",
  "name" : "MedicationAdministrationReasonnotgiven",
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
  "description" : "Reasons for not administering the medication",
  "code" : "reason-not-given",
  "base" : ["MedicationAdministration"],
  "type" : "token",
  "expression" : "MedicationAdministration.​statusReason"
}

```
