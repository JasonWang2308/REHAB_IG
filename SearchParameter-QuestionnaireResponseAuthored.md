# QuestionnaireResponseAuthored - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **QuestionnaireResponseAuthored**

## SearchParameter: QuestionnaireResponseAuthored 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/QuestionnaireResponse-authored | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:QuestionnaireResponseAuthored |

 
搜尋QuestionnaireResponse的authored參數 

## QuestionnaireResponseAuthored

Parameter `authored`:`date`

搜尋QuestionnaireResponse的authored參數

| | |
| :--- | :--- |
| Resource | [QuestionnaireResponse](http://hl7.org/fhir/R4/questionnaireresponse.html) |
| Expression | `QuestionnaireResponse.authored` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "QuestionnaireResponseAuthored",
  "url" : "http://example.org/fhir/SearchParameter/QuestionnaireResponse-authored",
  "version" : "0.1.0",
  "name" : "QuestionnaireResponseAuthored",
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
  "description" : "搜尋QuestionnaireResponse的authored參數",
  "code" : "authored",
  "base" : ["QuestionnaireResponse"],
  "type" : "date",
  "expression" : "QuestionnaireResponse.authored"
}

```
