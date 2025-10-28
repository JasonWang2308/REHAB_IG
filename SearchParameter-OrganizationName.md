# OrganizationName - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **OrganizationName**

## SearchParameter: OrganizationName 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Organization-name | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:OrganizationName |

 
搜尋Organization的name參數 

## OrganizationName

Parameter `name`:`string`

搜尋Organization的name參數

| | |
| :--- | :--- |
| Resource | [Organization](http://hl7.org/fhir/R4/organization.html) |
| Expression | `Organization.name` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "OrganizationName",
  "url" : "http://example.org/fhir/SearchParameter/Organization-name",
  "version" : "0.1.0",
  "name" : "OrganizationName",
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
  "description" : "搜尋Organization的name參數",
  "code" : "name",
  "base" : ["Organization"],
  "type" : "string",
  "expression" : "Organization.name"
}

```
