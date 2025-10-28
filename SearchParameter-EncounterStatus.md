# EncounterStatus - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **EncounterStatus**

## SearchParameter: EncounterStatus 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Encounter-status | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:EncounterStatus |

 
搜尋Encounter的status參數 

## EncounterStatus

Parameter `status`:`token`

搜尋Encounter的status參數

| | |
| :--- | :--- |
| Resource | [Encounter](http://hl7.org/fhir/R4/encounter.html) |
| Expression | `Encounter.status` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "EncounterStatus",
  "url" : "http://example.org/fhir/SearchParameter/Encounter-status",
  "version" : "0.1.0",
  "name" : "EncounterStatus",
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
  "description" : "搜尋Encounter的status參數",
  "code" : "status",
  "base" : ["Encounter"],
  "type" : "token",
  "expression" : "Encounter.status"
}

```
