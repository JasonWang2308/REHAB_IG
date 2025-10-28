# EncounterId - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **EncounterId**

## SearchParameter: EncounterId 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Encounter-_id | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:EncounterId |

 
搜尋Encounter的_id參數 

## EncounterId

Parameter `_id`:`token`

搜尋Encounter的_id參數

| | |
| :--- | :--- |
| Resource | [Encounter](http://hl7.org/fhir/R4/encounter.html) |
| Expression | `Encounter.id` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "EncounterId",
  "url" : "http://example.org/fhir/SearchParameter/Encounter-_id",
  "version" : "0.1.0",
  "name" : "EncounterId",
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
  "description" : "搜尋Encounter的_id參數",
  "code" : "_id",
  "base" : ["Encounter"],
  "type" : "token",
  "expression" : "Encounter.id"
}

```
