# MMSE QuestionnaireResponse (scored) - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MMSE QuestionnaireResponse (scored)**

## Resource Profile: MMSE QuestionnaireResponse (scored) 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/MMSEQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:MMSEQuestionnaireResponse |

 
MMSE 回覆：分數題逐題填答，總分需等於所有分數項目加總。 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)
* Examples for this Profile: [QuestionnaireResponse/MMSEQuestionnaireResponseExample](QuestionnaireResponse-MMSEQuestionnaireResponseExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/MMSEQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-MMSEQuestionnaireResponse.csv), [Excel](StructureDefinition-MMSEQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-MMSEQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "MMSEQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/MMSEQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "MMSEQuestionnaireResponse",
  "title" : "MMSE QuestionnaireResponse (scored)",
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
  "description" : "MMSE 回覆：分數題逐題填答，總分需等於所有分數項目加總。",
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
  "baseDefinition" : "http://example.org/StructureDefinition/SPACQuestionnaireResponse",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "QuestionnaireResponse",
        "path" : "QuestionnaireResponse",
        "constraint" : [
          {
            "key" : "mmse-total-check",
            "severity" : "error",
            "human" : "總分 (total-score) 必須等於所有 _score 題目的加總",
            "expression" : "item.where(linkId='total-score').answer.valueInteger = item.descendants().where(linkId.endsWith('_score') or linkId.contains('-score')).answer.valueInteger.sum()",
            "source" : "http://example.org/StructureDefinition/MMSEQuestionnaireResponse"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.status",
        "path" : "QuestionnaireResponse.status",
        "patternCode" : "completed"
      },
      {
        "id" : "QuestionnaireResponse.subject",
        "path" : "QuestionnaireResponse.subject",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : ["http://example.org/StructureDefinition/Patient"]
          }
        ]
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
          "rules" : "open"
        },
        "min" : 7
      },
      {
        "id" : "QuestionnaireResponse.item:section-1",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "section-1",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:section-1.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-1.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:section-1.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-1.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:section-1.item",
        "path" : "QuestionnaireResponse.item.item",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-1.item.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-2",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "section-2",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:section-2.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-2.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:section-2.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-2.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:section-2.item",
        "path" : "QuestionnaireResponse.item.item",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-2.item.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-3",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "section-3",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:section-3.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-3.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:section-3.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-3.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:section-3.item",
        "path" : "QuestionnaireResponse.item.item",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-3.item.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-4",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "section-4",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:section-4.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-4.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:section-4.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-4.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:section-4.item",
        "path" : "QuestionnaireResponse.item.item",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-4.item.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-5",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "section-5",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:section-5.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-5.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:section-5.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-5.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:section-5.item",
        "path" : "QuestionnaireResponse.item.item",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-5.item.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-6",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "section-6",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:section-6.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-6.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:section-6.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:section-6.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:section-6.item",
        "path" : "QuestionnaireResponse.item.item",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:section-6.item.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:total-score",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "total-score",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:total-score.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:total-score.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:total-score.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "total-score-mmse"
      },
      {
        "id" : "QuestionnaireResponse.item:total-score.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:total-score.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:total-score.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:total-score.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ]
      }
    ]
  }
}

```
