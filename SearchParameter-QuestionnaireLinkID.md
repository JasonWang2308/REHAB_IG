# QuestionnaireLinkID - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **QuestionnaireLinkID**

## SearchParameter: QuestionnaireLinkID 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/SearchParameter/Questionnaire-LinkID | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:QuestionnaireLinkID |

 
問卷項目 

## QuestionnaireLinkID

Parameter `LinkID`:`string`

問卷項目

| | |
| :--- | :--- |
| Resource | [Questionnaire](http://hl7.org/fhir/R4/questionnaire.html) |
| Expression | (none) |
| Multiples | * multipleAnd: It's up to the server whether the parameter may repeat in order to specify multiple values that must all be true
* multipleOr: It's up to the server whether the parameter can have multiple values (separated by comma) where at least one must be true
 |



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "QuestionnaireLinkID",
  "url" : "http://example.org/fhir/SearchParameter/Questionnaire-LinkID",
  "version" : "0.1.0",
  "name" : "QuestionnaireLinkID",
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
  "description" : "問卷項目",
  "code" : "LinkID",
  "base" : ["Questionnaire"],
  "type" : "string"
}

```
