# ConditionOnsetdate - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ConditionOnsetdate**

## SearchParameter: ConditionOnsetdate 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Condition-onset-date | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:ConditionOnsetdate |

 
搜尋Condition的onset-date參數 

## ConditionOnsetdate

Parameter `onset-date`:`date`

搜尋Condition的onset-date參數

| | |
| :--- | :--- |
| Resource | [Condition](http://hl7.org/fhir/R4/condition.html) |
| Expression | `Condition.onset.as(dateTime)|Condition.onset.as(Period)` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "ConditionOnsetdate",
  "url" : "http://example.org/fhir/SearchParameter/Condition-onset-date",
  "version" : "0.1.0",
  "name" : "ConditionOnsetdate",
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
  "description" : "搜尋Condition的onset-date參數",
  "code" : "onset-date",
  "base" : ["Condition"],
  "type" : "date",
  "expression" : "Condition.onset.as(dateTime)|Condition.onset.as(Period)"
}

```
