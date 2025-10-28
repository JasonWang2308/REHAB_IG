# QuestionnaireResponseQuestionnaire - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **QuestionnaireResponseQuestionnaire**

## SearchParameter: QuestionnaireResponseQuestionnaire 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/QuestionnaireResponse-questionnaire | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:QuestionnaireResponseQuestionnaire |

 
搜尋QuestionnaireResponse的questionnaire參數 

## QuestionnaireResponseQuestionnaire

Parameter `questionnaire`:`reference`

搜尋QuestionnaireResponse的questionnaire參數

| | |
| :--- | :--- |
| Resource | [QuestionnaireResponse](http://hl7.org/fhir/R4/questionnaireresponse.html) |
| Expression | `QuestionnaireResponse.questionnaire` |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "QuestionnaireResponseQuestionnaire",
  "url" : "http://example.org/fhir/SearchParameter/QuestionnaireResponse-questionnaire",
  "version" : "0.1.0",
  "name" : "QuestionnaireResponseQuestionnaire",
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
  "description" : "搜尋QuestionnaireResponse的questionnaire參數",
  "code" : "questionnaire",
  "base" : ["QuestionnaireResponse"],
  "type" : "reference",
  "expression" : "QuestionnaireResponse.questionnaire"
}

```
