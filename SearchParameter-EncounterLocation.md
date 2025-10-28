# EncounterLocation - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **EncounterLocation**

## SearchParameter: EncounterLocation 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Encounter-location | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:EncounterLocation |

 
搜尋Encounter的location參數 

## EncounterLocation

Parameter `location`:`reference`

搜尋Encounter的location參數

| | |
| :--- | :--- |
| Resource | [Encounter](http://hl7.org/fhir/R4/encounter.html) |
| Expression | `Encounter.location` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "EncounterLocation",
  "url" : "http://example.org/fhir/SearchParameter/Encounter-location",
  "version" : "0.1.0",
  "name" : "EncounterLocation",
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
  "description" : "搜尋Encounter的location參數",
  "code" : "location",
  "base" : ["Encounter"],
  "type" : "reference",
  "expression" : "Encounter.location"
}

```
