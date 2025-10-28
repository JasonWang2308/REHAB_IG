# GoalDescription - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **GoalDescription**

## SearchParameter: GoalDescription 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Goal-description | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:GoalDescription |

 
搜尋Goal的description參數 

## GoalDescription

Parameter `description`:`token`

搜尋Goal的description參數

| | |
| :--- | :--- |
| Resource | [Goal](http://hl7.org/fhir/R4/goal.html) |
| Expression | `Goal.description` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "GoalDescription",
  "url" : "http://example.org/fhir/SearchParameter/Goal-description",
  "version" : "0.1.0",
  "name" : "GoalDescription",
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
  "description" : "搜尋Goal的description參數",
  "code" : "description",
  "base" : ["Goal"],
  "type" : "token",
  "expression" : "Goal.description"
}

```
