# BundleIdentifier - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **BundleIdentifier**

## SearchParameter: BundleIdentifier 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Bundle-identifier | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:BundleIdentifier |

 
搜尋Bundle的identifier參數 

## BundleIdentifier

Parameter `identifier`:`token`

搜尋Bundle的identifier參數

| | |
| :--- | :--- |
| Resource | [Bundle](http://hl7.org/fhir/R4/bundle.html) |
| Expression | `Bundle.identifier` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "BundleIdentifier",
  "url" : "http://example.org/fhir/SearchParameter/Bundle-identifier",
  "version" : "0.1.0",
  "name" : "BundleIdentifier",
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
  "description" : "搜尋Bundle的identifier參數",
  "code" : "identifier",
  "base" : ["Bundle"],
  "type" : "token",
  "expression" : "Bundle.identifier"
}

```
