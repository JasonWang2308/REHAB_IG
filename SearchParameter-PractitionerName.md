# PractitionerName - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PractitionerName**

## SearchParameter: PractitionerName 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Practitioner-name | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:PractitionerName |

 
搜尋Practitioner的name參數 

## PractitionerName

Parameter `name`:`string`

搜尋Practitioner的name參數

| | |
| :--- | :--- |
| Resource | [Practitioner](http://hl7.org/fhir/R4/practitioner.html) |
| Expression | `Practitioner.name` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "PractitionerName",
  "url" : "http://example.org/fhir/SearchParameter/Practitioner-name",
  "version" : "0.1.0",
  "name" : "PractitionerName",
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
  "description" : "搜尋Practitioner的name參數",
  "code" : "name",
  "base" : ["Practitioner"],
  "type" : "string",
  "expression" : "Practitioner.name"
}

```
