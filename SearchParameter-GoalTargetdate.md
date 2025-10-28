# GoalTargetdate - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **GoalTargetdate**

## SearchParameter: GoalTargetdate 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Goal-target-date | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:GoalTargetdate |

 
搜尋Goal的target-date參數 

## GoalTargetdate

Parameter `target-date`:`date`

搜尋Goal的target-date參數

| | |
| :--- | :--- |
| Resource | [Goal](http://hl7.org/fhir/R4/goal.html) |
| Expression | `(Goal.target.due.ofType(date))` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "GoalTargetdate",
  "url" : "http://example.org/fhir/SearchParameter/Goal-target-date",
  "version" : "0.1.0",
  "name" : "GoalTargetdate",
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
  "description" : "搜尋Goal的target-date參數",
  "code" : "target-date",
  "base" : ["Goal"],
  "type" : "date",
  "expression" : "(Goal.target.due.ofType(date))"
}

```
