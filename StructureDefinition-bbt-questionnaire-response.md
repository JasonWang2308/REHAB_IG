# BBTQR - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **BBTQR**

## Resource Profile: BBTQR 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/bbt-questionnaire-response | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:BBTQR |

 
Box and Block Test (BBT) 評估量表問卷回覆 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)
* Examples for this Profile: [QuestionnaireResponse/BBTExample](QuestionnaireResponse-BBTExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/bbt-questionnaire-response)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-bbt-questionnaire-response.csv), [Excel](StructureDefinition-bbt-questionnaire-response.xlsx), [Schematron](StructureDefinition-bbt-questionnaire-response.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "bbt-questionnaire-response",
  "url" : "http://example.org/StructureDefinition/bbt-questionnaire-response",
  "version" : "0.1.0",
  "name" : "BBTQR",
  "status" : "draft",
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
  "description" : "Box and Block Test (BBT) 評估量表問卷回覆",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "workflow",
      "uri" : "http://hl7.org/fhir/workflow",
      "name" : "Workflow Pattern"
    },
    {
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    },
    {
      "identity" : "w5",
      "uri" : "http://hl7.org/fhir/fivews",
      "name" : "FiveWs Pattern Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "QuestionnaireResponse",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/QuestionnaireResponse",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "QuestionnaireResponse.questionnaire",
        "path" : "QuestionnaireResponse.questionnaire",
        "min" : 1,
        "patternCanonical" : "http://example.org/Questionnaire/BBTQuestionnaire",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.status",
        "path" : "QuestionnaireResponse.status",
        "fixedCode" : "completed",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item",
        "path" : "QuestionnaireResponse.item",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "linkId"
            }
          ],
          "rules" : "closed"
        },
        "min" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:left-hand",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "left-hand",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:left-hand.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "left-hand"
      },
      {
        "id" : "QuestionnaireResponse.item:right-hand",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "right-hand",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:right-hand.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "right-hand"
      }
    ]
  }
}

```
