# IADL評估問卷回覆 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **IADL評估問卷回覆**

## Resource Profile: IADL評估問卷回覆 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/IADLQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:IADLQuestionnaireResponse |

 
針對IADL評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/IADLQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-IADLQuestionnaireResponse.csv), [Excel](StructureDefinition-IADLQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-IADLQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "IADLQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/IADLQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "IADLQuestionnaireResponse",
  "title" : "IADL評估問卷回覆",
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
  "description" : "針對IADL評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構",
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
        "path" : "QuestionnaireResponse"
      },
      {
        "id" : "QuestionnaireResponse.questionnaire",
        "path" : "QuestionnaireResponse.questionnaire",
        "fixedCanonical" : "http://example.org/fhir/Questionnaire/IDALQuestionnaireInstance"
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
          "description" : "根據linkId區分IADL問卷的主要區塊",
          "ordered" : false,
          "rules" : "closed"
        },
        "min" : 9
      },
      {
        "id" : "QuestionnaireResponse.item:F1",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "F1",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:F1.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F1.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:F1.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "A-telephone"
      },
      {
        "id" : "QuestionnaireResponse.item:F1.text",
        "path" : "QuestionnaireResponse.item.text",
        "min" : 1,
        "patternString" : "A.使用電話"
      },
      {
        "id" : "QuestionnaireResponse.item:F1.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1",
        "minValueInteger" : 1,
        "maxValueInteger" : 4
      },
      {
        "id" : "QuestionnaireResponse.item:F1.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F1.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:F1.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "min" : 1,
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:F2",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "F2",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:F2.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F2.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:F2.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "patternString" : "B-shopping"
      },
      {
        "id" : "QuestionnaireResponse.item:F2.text",
        "path" : "QuestionnaireResponse.item.text",
        "min" : 1,
        "patternString" : "B.購物"
      },
      {
        "id" : "QuestionnaireResponse.item:F2.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1",
        "minValueInteger" : 1,
        "maxValueInteger" : 4
      },
      {
        "id" : "QuestionnaireResponse.item:F2.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F2.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:F2.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "min" : 1,
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:F3",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "F3",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:F3.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F3.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:F3.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "patternString" : "C-food-preparation"
      },
      {
        "id" : "QuestionnaireResponse.item:F3.text",
        "path" : "QuestionnaireResponse.item.text",
        "min" : 1,
        "patternString" : "C.備餐"
      },
      {
        "id" : "QuestionnaireResponse.item:F3.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1",
        "minValueInteger" : 1,
        "maxValueInteger" : 4
      },
      {
        "id" : "QuestionnaireResponse.item:F3.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F3.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:F3.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "min" : 1,
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:F4",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "F4",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:F4.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F4.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:F4.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "patternString" : "D-housekeeping"
      },
      {
        "id" : "QuestionnaireResponse.item:F4.text",
        "path" : "QuestionnaireResponse.item.text",
        "min" : 1,
        "patternString" : "D.處理家務"
      },
      {
        "id" : "QuestionnaireResponse.item:F4.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1",
        "minValueInteger" : 1,
        "maxValueInteger" : 4
      },
      {
        "id" : "QuestionnaireResponse.item:F4.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F4.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:F4.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "min" : 1,
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:F5",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "F5",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:F5.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F5.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:F5.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "patternString" : "E-laundry"
      },
      {
        "id" : "QuestionnaireResponse.item:F5.text",
        "path" : "QuestionnaireResponse.item.text",
        "min" : 1,
        "patternString" : "E.洗衣服"
      },
      {
        "id" : "QuestionnaireResponse.item:F5.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1",
        "minValueInteger" : 1,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:F5.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F5.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:F5.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "min" : 1,
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:F6",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "F6",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:F6.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F6.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:F6.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "patternString" : "F-transportation"
      },
      {
        "id" : "QuestionnaireResponse.item:F6.text",
        "path" : "QuestionnaireResponse.item.text",
        "min" : 1,
        "patternString" : "F.外出"
      },
      {
        "id" : "QuestionnaireResponse.item:F6.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1",
        "minValueInteger" : 1,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:F6.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F6.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:F6.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "min" : 1,
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:F7",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "F7",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:F7.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F7.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:F7.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "patternString" : "G-medications"
      },
      {
        "id" : "QuestionnaireResponse.item:F7.text",
        "path" : "QuestionnaireResponse.item.text",
        "min" : 1,
        "patternString" : "G.服用藥物"
      },
      {
        "id" : "QuestionnaireResponse.item:F7.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1",
        "minValueInteger" : 1,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:F7.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F7.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:F7.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "min" : 1,
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:F8",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "F8",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:F8.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F8.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:F8.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "patternString" : "H-finances"
      },
      {
        "id" : "QuestionnaireResponse.item:F8.text",
        "path" : "QuestionnaireResponse.item.text",
        "min" : 1,
        "patternString" : "H.處理財務的能力"
      },
      {
        "id" : "QuestionnaireResponse.item:F8.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1",
        "minValueInteger" : 1,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:F8.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:F8.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:F8.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "min" : 1,
        "type" : [
          {
            "code" : "integer"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "totalScoreSection",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "I-total-score-IADL"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "I.IADL總分計算"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 8,
        "maxValueInteger" : 30
      }
    ]
  }
}

```
