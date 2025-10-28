# PatientBirthdate - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PatientBirthdate**

## SearchParameter: PatientBirthdate 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Patient-birthdate | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:PatientBirthdate |

 
搜尋Patient的birthdate參數 

## PatientBirthdate

Parameter `birthdate`:`date`

搜尋Patient的birthdate參數

| | |
| :--- | :--- |
| Resource | [Patient](http://hl7.org/fhir/R4/patient.html) |
| Expression | `Patient.birthDate` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "PatientBirthdate",
  "url" : "http://example.org/fhir/SearchParameter/Patient-birthdate",
  "version" : "0.1.0",
  "name" : "PatientBirthdate",
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
  "description" : "搜尋Patient的birthdate參數",
  "code" : "birthdate",
  "base" : ["Patient"],
  "type" : "date",
  "expression" : "Patient.birthDate"
}

```
