# ProcedureStatus - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ProcedureStatus**

## SearchParameter: ProcedureStatus 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Procedure-status | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:ProcedureStatus |

 
搜尋Procedure的status參數 

## ProcedureStatus

Parameter `status`:`token`

搜尋Procedure的status參數

| | |
| :--- | :--- |
| Resource | [Procedure](http://hl7.org/fhir/R4/procedure.html) |
| Expression | `Procedure.status` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "ProcedureStatus",
  "url" : "http://example.org/fhir/SearchParameter/Procedure-status",
  "version" : "0.1.0",
  "name" : "ProcedureStatus",
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
  "description" : "搜尋Procedure的status參數",
  "code" : "status",
  "base" : ["Procedure"],
  "type" : "token",
  "expression" : "Procedure.status"
}

```
