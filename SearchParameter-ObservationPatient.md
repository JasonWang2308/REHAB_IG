# ObservationPatient - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ObservationPatient**

## SearchParameter: ObservationPatient 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Observation-patient | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:ObservationPatient |

 
搜尋Observation的patient參數 

## ObservationPatient

Parameter `patient`:`reference`

搜尋Observation的patient參數

| | |
| :--- | :--- |
| Resource | [Observation](http://hl7.org/fhir/R4/observation.html) |
| Expression | `Observation.subject.where(resolve() is Patient)` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "ObservationPatient",
  "url" : "http://example.org/fhir/SearchParameter/Observation-patient",
  "version" : "0.1.0",
  "name" : "ObservationPatient",
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
  "description" : "搜尋Observation的patient參數",
  "code" : "patient",
  "base" : ["Observation"],
  "type" : "reference",
  "expression" : "Observation.subject.where(resolve() is Patient)"
}

```
