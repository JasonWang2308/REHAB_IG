# QuestionnaireResponsePatient - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **QuestionnaireResponsePatient**

## SearchParameter: QuestionnaireResponsePatient 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/QuestionnaireResponse-patient | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:QuestionnaireResponsePatient |

 
搜尋QuestionnaireResponse的patient參數 

## QuestionnaireResponsePatient

Parameter `patient`:`reference`

搜尋QuestionnaireResponse的patient參數

| | |
| :--- | :--- |
| Resource | [QuestionnaireResponse](http://hl7.org/fhir/R4/questionnaireresponse.html) |
| Expression | `QuestionnaireResponse.subject.where(resolve() is Patient)` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "QuestionnaireResponsePatient",
  "url" : "http://example.org/fhir/SearchParameter/QuestionnaireResponse-patient",
  "version" : "0.1.0",
  "name" : "QuestionnaireResponsePatient",
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
  "description" : "搜尋QuestionnaireResponse的patient參數",
  "code" : "patient",
  "base" : ["QuestionnaireResponse"],
  "type" : "reference",
  "expression" : "QuestionnaireResponse.subject.where(resolve() is Patient)"
}

```
