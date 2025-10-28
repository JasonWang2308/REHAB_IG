# MedicationAdministrationCode - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationAdministrationCode**

## SearchParameter: MedicationAdministrationCode 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/MedicationAdministration-code | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:MedicationAdministrationCode |

 
Return administrations of this medication code 

## MedicationAdministrationCode

Parameter `code`:`token`

Return administrations of this medication code

| | |
| :--- | :--- |
| Resource | [MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) |
| Expression | `(MedicationAdministration.​medication as CodeableConcept)` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "MedicationAdministrationCode",
  "url" : "http://example.org/fhir/SearchParameter/MedicationAdministration-code",
  "version" : "0.1.0",
  "name" : "MedicationAdministrationCode",
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
  "description" : "Return administrations of this medication code",
  "code" : "code",
  "base" : ["MedicationAdministration"],
  "type" : "token",
  "expression" : "(MedicationAdministration.​medication as CodeableConcept)"
}

```
