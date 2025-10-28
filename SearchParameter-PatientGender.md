# PatientGender - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PatientGender**

## SearchParameter: PatientGender 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Patient-gender | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:PatientGender |

 
搜尋Patient的gender參數 

## PatientGender

Parameter `gender`:`token`

搜尋Patient的gender參數

| | |
| :--- | :--- |
| Resource | [Patient](http://hl7.org/fhir/R4/patient.html) |
| Expression | `Patient.gender` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "PatientGender",
  "url" : "http://example.org/fhir/SearchParameter/Patient-gender",
  "version" : "0.1.0",
  "name" : "PatientGender",
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
  "description" : "搜尋Patient的gender參數",
  "code" : "gender",
  "base" : ["Patient"],
  "type" : "token",
  "expression" : "Patient.gender"
}

```
