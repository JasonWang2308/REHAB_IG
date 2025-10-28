# OrganizationType - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **OrganizationType**

## SearchParameter: OrganizationType 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Organization-type | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:OrganizationType |

 
搜尋Organization的type參數 

## OrganizationType

Parameter `type`:`token`

搜尋Organization的type參數

| | |
| :--- | :--- |
| Resource | [Organization](http://hl7.org/fhir/R4/organization.html) |
| Expression | `Organization.type` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "OrganizationType",
  "url" : "http://example.org/fhir/SearchParameter/Organization-type",
  "version" : "0.1.0",
  "name" : "OrganizationType",
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
  "description" : "搜尋Organization的type參數",
  "code" : "type",
  "base" : ["Organization"],
  "type" : "token",
  "expression" : "Organization.type"
}

```
