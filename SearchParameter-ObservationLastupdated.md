# ObservationLastupdated - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ObservationLastupdated**

## SearchParameter: ObservationLastupdated 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Observation-_lastUpdated | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:ObservationLastupdated |

 
搜尋Observation的_lastUpdated參數 

## ObservationLastupdated

Parameter `_lastUpdated`:`date`

搜尋Observation的_lastUpdated參數

| | |
| :--- | :--- |
| Resource | [Observation](http://hl7.org/fhir/R4/observation.html) |
| Expression | `Resource.meta.lastUpdated` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "ObservationLastupdated",
  "url" : "http://example.org/fhir/SearchParameter/Observation-_lastUpdated",
  "version" : "0.1.0",
  "name" : "ObservationLastupdated",
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
  "description" : "搜尋Observation的_lastUpdated參數",
  "code" : "_lastUpdated",
  "base" : ["Observation"],
  "type" : "date",
  "expression" : "Resource.meta.lastUpdated"
}

```
