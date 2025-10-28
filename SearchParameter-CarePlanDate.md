# CarePlanDate - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **CarePlanDate**

## SearchParameter: CarePlanDate 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/CarePlan-date | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:CarePlanDate |

 
搜尋CarePlan的date參數 

## CarePlanDate

Parameter `date`:`date`

搜尋CarePlan的date參數

| | |
| :--- | :--- |
| Resource | [CarePlan](http://hl7.org/fhir/R4/careplan.html) |
| Expression | `CarePlan.period` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "CarePlanDate",
  "url" : "http://example.org/fhir/SearchParameter/CarePlan-date",
  "version" : "0.1.0",
  "name" : "CarePlanDate",
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
  "description" : "搜尋CarePlan的date參數",
  "code" : "date",
  "base" : ["CarePlan"],
  "type" : "date",
  "expression" : "CarePlan.period"
}

```
