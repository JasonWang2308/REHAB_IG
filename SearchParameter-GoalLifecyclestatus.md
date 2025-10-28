# GoalLifecyclestatus - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **GoalLifecyclestatus**

## SearchParameter: GoalLifecyclestatus 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Goal-lifecycle-status | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:GoalLifecyclestatus |

 
搜尋Goal的lifecycle-status參數 

## GoalLifecyclestatus

Parameter `lifecycle-status`:`token`

搜尋Goal的lifecycle-status參數

| | |
| :--- | :--- |
| Resource | [Goal](http://hl7.org/fhir/R4/goal.html) |
| Expression | `Goal.lifecycleStatus` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "GoalLifecyclestatus",
  "url" : "http://example.org/fhir/SearchParameter/Goal-lifecycle-status",
  "version" : "0.1.0",
  "name" : "GoalLifecyclestatus",
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
  "description" : "搜尋Goal的lifecycle-status參數",
  "code" : "lifecycle-status",
  "base" : ["Goal"],
  "type" : "token",
  "expression" : "Goal.lifecycleStatus"
}

```
