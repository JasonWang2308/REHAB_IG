# PractitionerRoleSpecialty - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PractitionerRoleSpecialty**

## SearchParameter: PractitionerRoleSpecialty 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/PractitionerRole-specialty | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:PractitionerRoleSpecialty |

 
搜尋PractitionerRole的specialty參數 

## PractitionerRoleSpecialty

Parameter `specialty`:`token`

搜尋PractitionerRole的specialty參數

| | |
| :--- | :--- |
| Resource | [PractitionerRole](http://hl7.org/fhir/R4/practitionerrole.html) |
| Expression | `PractitionerRole.specialty` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "PractitionerRoleSpecialty",
  "url" : "http://example.org/fhir/SearchParameter/PractitionerRole-specialty",
  "version" : "0.1.0",
  "name" : "PractitionerRoleSpecialty",
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
  "description" : "搜尋PractitionerRole的specialty參數",
  "code" : "specialty",
  "base" : ["PractitionerRole"],
  "type" : "token",
  "expression" : "PractitionerRole.specialty"
}

```
