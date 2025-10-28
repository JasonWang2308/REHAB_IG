# ConditionAbatementdate - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ConditionAbatementdate**

## SearchParameter: ConditionAbatementdate 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Condition-abatement-date | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:ConditionAbatementdate |

 
搜尋Condition的abatement-date參數 

## ConditionAbatementdate

Parameter `abatement-date`:`date`

搜尋Condition的abatement-date參數

| | |
| :--- | :--- |
| Resource | [Condition](http://hl7.org/fhir/R4/condition.html) |
| Expression | `Condition.abatement.as(dateTime)` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "ConditionAbatementdate",
  "url" : "http://example.org/fhir/SearchParameter/Condition-abatement-date",
  "version" : "0.1.0",
  "name" : "ConditionAbatementdate",
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
  "description" : "搜尋Condition的abatement-date參數",
  "code" : "abatement-date",
  "base" : ["Condition"],
  "type" : "date",
  "expression" : "Condition.abatement.as(dateTime)"
}

```
