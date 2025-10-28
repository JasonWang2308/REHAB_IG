# CarePlanCategory - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **CarePlanCategory**

## SearchParameter: CarePlanCategory 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/CarePlan-category | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:CarePlanCategory |

 
搜尋CarePlan的category參數 

## CarePlanCategory

Parameter `category`:`token`

搜尋CarePlan的category參數

| | |
| :--- | :--- |
| Resource | [CarePlan](http://hl7.org/fhir/R4/careplan.html) |
| Expression | `CarePlan.category` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "CarePlanCategory",
  "url" : "http://example.org/fhir/SearchParameter/CarePlan-category",
  "version" : "0.1.0",
  "name" : "CarePlanCategory",
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
  "description" : "搜尋CarePlan的category參數",
  "code" : "category",
  "base" : ["CarePlan"],
  "type" : "token",
  "expression" : "CarePlan.category"
}

```
