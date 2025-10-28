# 巴氏量表問卷回覆 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **巴氏量表問卷回覆**

## Resource Profile: 巴氏量表問卷回覆 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/BarthelQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:BarthelQuestionnaireResponse |

 
針對巴氏量表問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)
* Examples for this Profile: [QuestionnaireResponse/BarthelIndexExample](QuestionnaireResponse-BarthelIndexExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/BarthelQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-BarthelQuestionnaireResponse.csv), [Excel](StructureDefinition-BarthelQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-BarthelQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BarthelQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/BarthelQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "BarthelQuestionnaireResponse",
  "title" : "巴氏量表問卷回覆",
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
  "description" : "針對巴氏量表問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構",
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
        "patternCanonical" : "http://example.org/Questionnaire/BarthelQuestionnaireInstance"
      },
      {
        "id" : "QuestionnaireResponse.status",
        "path" : "QuestionnaireResponse.status",
        "fixedCode" : "completed"
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
        "min" : 11
      },
      {
        "id" : "QuestionnaireResponse.item:feeding",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "feeding",
        "short" : "進食分數 對應到LOINC代碼",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:feeding.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:feeding.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:feeding.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "A-feeding"
      },
      {
        "id" : "QuestionnaireResponse.item:feeding.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "進食 (Feeding)"
      },
      {
        "id" : "QuestionnaireResponse.item:feeding.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:feeding.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:feeding.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:feeding.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelFeeding"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:grooming",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "grooming",
        "short" : "穿脫衣服分數 對應到LOINC代碼",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:grooming.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:grooming.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:grooming.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "B-grooming"
      },
      {
        "id" : "QuestionnaireResponse.item:grooming.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "個人衛生 (Grooming)"
      },
      {
        "id" : "QuestionnaireResponse.item:grooming.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:grooming.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:grooming.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:grooming.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelGrooming"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:toiletuse",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "toiletuse",
        "short" : "上廁所分數 對應到LOINC代碼",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:toiletuse.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:toiletuse.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:toiletuse.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "C-toilet Use"
      },
      {
        "id" : "QuestionnaireResponse.item:toiletuse.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "上廁所 (Toilet Use)"
      },
      {
        "id" : "QuestionnaireResponse.item:toiletuse.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:toiletuse.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:toiletuse.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:toiletuse.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelToiletUse"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:bathing",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "bathing",
        "short" : "洗澡分數 對應到LOINC代碼",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:bathing.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:bathing.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:bathing.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "D-bathing"
      },
      {
        "id" : "QuestionnaireResponse.item:bathing.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "洗澡 (Bathing)"
      },
      {
        "id" : "QuestionnaireResponse.item:bathing.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:bathing.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:bathing.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:bathing.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelBathing"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:dressing",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "dressing",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:dressing.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:dressing.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:dressing.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "E-dressing"
      },
      {
        "id" : "QuestionnaireResponse.item:dressing.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "穿脫衣服 (Dressing)"
      },
      {
        "id" : "QuestionnaireResponse.item:dressing.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:dressing.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:dressing.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:dressing.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelDressing"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:bowels",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "bowels",
        "short" : "大便控制分數 對應到LOINC代碼",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:bowels.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:bowels.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:bowels.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "F-bowels"
      },
      {
        "id" : "QuestionnaireResponse.item:bowels.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "大便控制 (Bowels)"
      },
      {
        "id" : "QuestionnaireResponse.item:bowels.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:bowels.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:bowels.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:bowels.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelBowels"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:bladder",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "bladder",
        "short" : "小便控制分數 對應到LOINC代碼",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:bladder.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:bladder.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:bladder.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "G-bladder"
      },
      {
        "id" : "QuestionnaireResponse.item:bladder.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "小便控制 (Bladder)"
      },
      {
        "id" : "QuestionnaireResponse.item:bladder.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:bladder.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:bladder.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:bladder.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelBladder"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:mobility",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "mobility",
        "short" : "平地行走分數 對應到LOINC代碼",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:mobility.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:mobility.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:mobility.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "H-mobility"
      },
      {
        "id" : "QuestionnaireResponse.item:mobility.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "平地行走 (Mobility)"
      },
      {
        "id" : "QuestionnaireResponse.item:mobility.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:mobility.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:mobility.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:mobility.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelMobility"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:stairs",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "stairs",
        "short" : "上下樓梯分數 對應到LOINC代碼",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:stairs.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:stairs.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:stairs.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "I-stairs"
      },
      {
        "id" : "QuestionnaireResponse.item:stairs.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "上下樓梯 (Stairs)"
      },
      {
        "id" : "QuestionnaireResponse.item:stairs.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:stairs.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:stairs.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:stairs.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelStairs"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:transfer",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "transfer",
        "short" : "移位分數 對應到LOINC代碼",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:transfer.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:transfer.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:transfer.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "J-transfer"
      },
      {
        "id" : "QuestionnaireResponse.item:transfer.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "移位(Transfer)"
      },
      {
        "id" : "QuestionnaireResponse.item:transfer.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:transfer.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:transfer.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:transfer.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/VSBarthelTransfer"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:total",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "total",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:total.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:total.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:total.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "K-total-score-Barthel"
      },
      {
        "id" : "QuestionnaireResponse.item:total.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "巴氏量表總分"
      },
      {
        "id" : "QuestionnaireResponse.item:total.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:total.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:total.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:total.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 100
      }
    ]
  }
}

```
