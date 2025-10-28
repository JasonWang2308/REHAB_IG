# CarePlanPatient - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **CarePlanPatient**

## SearchParameter: CarePlanPatient 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/CarePlan-patient | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:CarePlanPatient |

 
搜尋CarePlan的patient參數 

## CarePlanPatient

Parameter `patient`:`reference`

搜尋CarePlan的patient參數

| | |
| :--- | :--- |
| Resource | [CarePlan](http://hl7.org/fhir/R4/careplan.html) |
| Expression | `CarePlan.subject.where(resolve() is Patient)` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "CarePlanPatient",
  "url" : "http://example.org/fhir/SearchParameter/CarePlan-patient",
  "version" : "0.1.0",
  "name" : "CarePlanPatient",
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
  "description" : "搜尋CarePlan的patient參數",
  "code" : "patient",
  "base" : ["CarePlan"],
  "type" : "reference",
  "expression" : "CarePlan.subject.where(resolve() is Patient)"
}

```
