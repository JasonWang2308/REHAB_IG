# ARAT上肢功能評估問卷回覆 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ARAT上肢功能評估問卷回覆**

## Resource Profile: ARAT上肢功能評估問卷回覆 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/ARATQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:ARATQuestionnaireResponse |

 
針對ARAT上肢功能評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)
* Examples for this Profile: [QuestionnaireResponse/arat-response-example-001](QuestionnaireResponse-arat-response-example-001.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/ARATQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ARATQuestionnaireResponse.csv), [Excel](StructureDefinition-ARATQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-ARATQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ARATQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/ARATQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "ARATQuestionnaireResponse",
  "title" : "ARAT上肢功能評估問卷回覆",
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
  "description" : "針對ARAT上肢功能評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構",
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
        "fixedCanonical" : "http://example.org/fhir/Questionnaire/ARATQuestionnaireInstance"
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
          "description" : "根據linkId區分ARAT問卷的主要區塊",
          "ordered" : false,
          "rules" : "closed"
        },
        "min" : 6
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentSide",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "assessmentSide",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentSide.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentSide.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentSide.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "assessment-side-arat"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentSide.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "請選擇評估側"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentSide.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentSide.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentSide.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentSide.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/assessment-side-valueset"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "graspSubscale",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "A-grasp-subscale"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "A.抓力分量表"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item",
        "path" : "QuestionnaireResponse.item.item",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "linkId"
            }
          ],
          "rules" : "closed"
        },
        "min" : 7
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock10cm3",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aBlock10cm3",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock10cm3.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock10cm3.extension:testTimeA1",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeA1",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock10cm3.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-block-10cm3"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock10cm3.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "方塊積木, 10 立方公分"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock10cm3.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock10cm3.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock2_5cm3",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aBlock2_5cm3",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock2_5cm3.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock2_5cm3.extension:testTimeA2",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeA2",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock2_5cm3.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-block-2.5cm3"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock2_5cm3.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "方塊積木, 2.5 立方公分"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock2_5cm3.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock2_5cm3.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock5cm3",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aBlock5cm3",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock5cm3.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock5cm3.extension:testTimeA3",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeA3",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock5cm3.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-block-5cm3"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock5cm3.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "方塊積木, 5 立方公分"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock5cm3.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock5cm3.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock7_5cm3",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aBlock7_5cm3",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock7_5cm3.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock7_5cm3.extension:testTimeA4",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeA4",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock7_5cm3.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-block-7.5cm3"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock7_5cm3.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "方塊積木, 7.5 立方公分"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock7_5cm3.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aBlock7_5cm3.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aCricketBall",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aCricketBall",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aCricketBall.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aCricketBall.extension:testTimeA5",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeA5",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aCricketBall.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-cricket-ball"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aCricketBall.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "板球"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aCricketBall.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aCricketBall.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aSharpeningStone",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aSharpeningStone",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aSharpeningStone.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aSharpeningStone.extension:testTimeA6",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeA6",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aSharpeningStone.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-sharpening-stone"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aSharpeningStone.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "磨刀石"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aSharpeningStone.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:aSharpeningStone.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:sectionASubscore",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "sectionASubscore",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:sectionASubscore.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-grasp-subscale-subscore"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:sectionASubscore.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "A.抓力分數"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:sectionASubscore.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:graspSubscale.item:sectionASubscore.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-18",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 18
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "gripSubscale",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "B-grip-subscale"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "B.握力分量表"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item",
        "path" : "QuestionnaireResponse.item.item",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "linkId"
            }
          ],
          "rules" : "closed"
        },
        "min" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPourWater",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bPourWater",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPourWater.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPourWater.extension:testTimeB1",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeB1",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPourWater.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-pour-water-from-one-glass-to-another"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPourWater.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "將水從一個杯子倒到另一個杯子"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPourWater.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPourWater.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace225cm",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bDisplace225cm",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace225cm.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace225cm.extension:testTimeB2",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeB2",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace225cm.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-pour-water-from-one-glass-to-another"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace225cm.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "將 2.25 公分合金管從桌子的一側移到另一側"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace225cm.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace225cm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace1cm",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bDisplace1cm",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace1cm.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace1cm.extension:testTimeB3",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeB3",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace1cm.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-displace-1-cm-alloy-tube-from-one-side-of-table-to-the-other"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace1cm.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "將 1 公分合金管從桌子的一側移到另一側"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace1cm.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bDisplace1cm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPutWasher",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bPutWasher",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPutWasher.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPutWasher.extension:testTimeB4",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeB4",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPutWasher.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-put-washer-over-bolt"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPutWasher.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "將墊圈放在螺栓上"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPutWasher.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:bPutWasher.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:sectionBSubscore",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "sectionBSubscore",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:sectionBSubscore.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-grip-subscale-subscore"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:sectionBSubscore.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "B.握力分數"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:sectionBSubscore.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:gripSubscale.item:sectionBSubscore.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-12",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 12
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "pinchSubscale",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "C-pinch-subscale"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "C.捏取分量表"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item",
        "path" : "QuestionnaireResponse.item.item",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "linkId"
            }
          ],
          "rules" : "closed"
        },
        "min" : 7
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingRing",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "cBallBearingRing",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingRing.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingRing.extension:testTimeC1",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeC1",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingRing.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-I-ball-bearing-held-between-ring-finger-and-thumb"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingRing.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "滾珠軸承，握在無名指與大拇指之間"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingRing.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingRing.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleIndex",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "cMarbleIndex",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleIndex.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleIndex.extension:testTimeC2",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeC2",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleIndex.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-I-marble-held-between-index-finger-and-thumb"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleIndex.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "大理石，握在食指與大拇指之間"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleIndex.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleIndex.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingMiddle",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "cBallBearingMiddle",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingMiddle.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingMiddle.extension:testTimeC3",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeC3",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingMiddle.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-I-ball-bearing-held-between-middle-finger-and-thumb"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingMiddle.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "滾珠軸承，握在中指與拇指之間"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingMiddle.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingMiddle.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingIndex",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "cBallBearingIndex",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingIndex.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingIndex.extension:testTimeC4",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeC4",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingIndex.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-I-ball-bearing-held-between-index-finger-and-thumb"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingIndex.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "滾珠軸承，握在食指與拇指之間"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingIndex.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cBallBearingIndex.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleRing",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "cMarbleRing",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleRing.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleRing.extension:testTimeC5",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeC5",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleRing.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-I-marble-held-between-ring-finger-and-thumb"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleRing.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "大理石，握在無名指和大拇指之間"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleRing.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleRing.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleMiddle",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "cMarbleMiddle",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleMiddle.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleMiddle.extension:testTimeC6",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeC6",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleMiddle.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-I-marble-held-between-middle-finger-and-thumb"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleMiddle.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "大理石，握在中指與大拇指之間"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleMiddle.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:cMarbleMiddle.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:sectionCSubscore",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "sectionCSubscore",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:sectionCSubscore.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-pinch-subscale-subscore"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:sectionCSubscore.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "C.捏取分數"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:sectionCSubscore.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:pinchSubscale.item:sectionCSubscore.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-18",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 18
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "grossMovementSubscale",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "D-gross-movement-subscale"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "D.粗大動作分量表"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item",
        "path" : "QuestionnaireResponse.item.item",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "linkId"
            }
          ],
          "rules" : "closed"
        },
        "min" : 4
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandBehindHead",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "dHandBehindHead",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandBehindHead.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandBehindHead.extension:testTimeD1",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeD1",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandBehindHead.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "D-I-hand-to-behind-the-head"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandBehindHead.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "手放在腦後"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandBehindHead.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandBehindHead.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandTopHead",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "dHandTopHead",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandTopHead.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandTopHead.extension:testTimeD2",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeD2",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandTopHead.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "D-I-hand-to-top-of-head"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandTopHead.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "手放在頭頂"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandTopHead.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandTopHead.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandMouth",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "dHandMouth",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandMouth.extension",
        "path" : "QuestionnaireResponse.item.item.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        },
        "short" : "完成時間（秒）"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandMouth.extension:testTimeD3",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeD3",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://example.org/StructureDefinition/test-time-extension"]
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandMouth.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "D-I-hand-to-mouth"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandMouth.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "手到嘴"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandMouth.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:dHandMouth.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-3",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:sectionDSubscore",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "sectionDSubscore",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:sectionDSubscore.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "D-gross-movement-subscale-subscore"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:sectionDSubscore.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "D.粗大動作分數"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:sectionDSubscore.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:grossMovementSubscale.item:sectionDSubscore.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-9",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 9
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
        "fixedString" : "E-total-score-ARAT"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "E.ARAT總分計算"
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
        "short" : "ARAT總分",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 57
      }
    ]
  }
}

```
