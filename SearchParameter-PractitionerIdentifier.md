# PractitionerIdentifier - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PractitionerIdentifier**

## SearchParameter: PractitionerIdentifier 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Practitioner-identifier | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:PractitionerIdentifier |

 
搜尋Practitioner的identifier參數 

## PractitionerIdentifier

Parameter `identifier`:`token`

搜尋Practitioner的identifier參數

| | |
| :--- | :--- |
| Resource | [Practitioner](http://hl7.org/fhir/R4/practitioner.html) |
| Expression | `Practitioner.identifier` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "PractitionerIdentifier",
  "url" : "http://example.org/fhir/SearchParameter/Practitioner-identifier",
  "version" : "0.1.0",
  "name" : "PractitionerIdentifier",
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
  "description" : "搜尋Practitioner的identifier參數",
  "code" : "identifier",
  "base" : ["Practitioner"],
  "type" : "token",
  "expression" : "Practitioner.identifier"
}

```
