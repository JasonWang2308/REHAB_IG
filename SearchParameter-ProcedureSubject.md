# ProcedureSubject - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ProcedureSubject**

## SearchParameter: ProcedureSubject 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Procedure-subject | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:ProcedureSubject |

 
搜尋Procedure的subject參數 

## ProcedureSubject

Parameter `subject`:`reference`

搜尋Procedure的subject參數

| | |
| :--- | :--- |
| Resource | [Procedure](http://hl7.org/fhir/R4/procedure.html) |
| Expression | `Procedure.subject` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "ProcedureSubject",
  "url" : "http://example.org/fhir/SearchParameter/Procedure-subject",
  "version" : "0.1.0",
  "name" : "ProcedureSubject",
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
  "description" : "搜尋Procedure的subject參數",
  "code" : "subject",
  "base" : ["Procedure"],
  "type" : "reference",
  "expression" : "Procedure.subject"
}

```
