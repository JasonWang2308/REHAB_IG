# ObservationStatus - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ObservationStatus**

## SearchParameter: ObservationStatus 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Observation-status | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:ObservationStatus |

 
搜尋Observation的status參數 

## ObservationStatus

Parameter `status`:`token`

搜尋Observation的status參數

| | |
| :--- | :--- |
| Resource | [Observation](http://hl7.org/fhir/R4/observation.html) |
| Expression | `Observation.status` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "ObservationStatus",
  "url" : "http://example.org/fhir/SearchParameter/Observation-status",
  "version" : "0.1.0",
  "name" : "ObservationStatus",
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
  "description" : "搜尋Observation的status參數",
  "code" : "status",
  "base" : ["Observation"],
  "type" : "token",
  "expression" : "Observation.status"
}

```
