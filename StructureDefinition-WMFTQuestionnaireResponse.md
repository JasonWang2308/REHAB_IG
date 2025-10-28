# WMFT上肢功能評估問卷回覆 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **WMFT上肢功能評估問卷回覆**

## Resource Profile: WMFT上肢功能評估問卷回覆 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/WMFTQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:WMFTQuestionnaireResponse |

 
針對WMFT上肢功能評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)
* Examples for this Profile: [QuestionnaireResponse/WMFTQuestionnaireResponseExample](QuestionnaireResponse-WMFTQuestionnaireResponseExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/WMFTQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-WMFTQuestionnaireResponse.csv), [Excel](StructureDefinition-WMFTQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-WMFTQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "WMFTQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/WMFTQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "WMFTQuestionnaireResponse",
  "title" : "WMFT上肢功能評估問卷回覆",
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
  "description" : "針對WMFT上肢功能評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構",
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
        "id" : "QuestionnaireResponse.questionnaire",
        "path" : "QuestionnaireResponse.questionnaire",
        "fixedCanonical" : "http://example.org/fhir/Questionnaire/WMFTQuestionnaireInstance"
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
          "description" : "根據linkId區分WMFT問卷的主要區塊",
          "ordered" : false,
          "rules" : "closed"
        },
        "min" : 4
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
        "fixedString" : "assessment-side-wmft"
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "TimedJointSegmentMovements",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "A-timed-joint-segment-movements"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "A.定時關節分段動作評估"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToTableSide",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aForearmToTableSide",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToTableSide.extension",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToTableSide.extension:testTimeA1",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToTableSide.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-forearm-to-table-side"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToTableSide.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "透過外展肩膀將前臂放在桌子上"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToTableSide.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToTableSide.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToBoxSide",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aForearmToBoxSide",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToBoxSide.extension",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToBoxSide.extension:testTimeA2",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToBoxSide.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-forearm-to-box-side"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToBoxSide.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "將前臂放在一個 25.4 公分高的箱子上，透過肩部外展"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToBoxSide.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aForearmToBoxSide.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowSide",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aExtendedElbowSide",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowSide.extension",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowSide.extension:testTimeA3",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowSide.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-extended-elbow-side"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowSide.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "將手肘伸向一側，越過一張 28 公分長的桌子"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowSide.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowSide.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowToTheSideWith1lbWeight",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aExtendedElbowToTheSideWith1lbWeight",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowToTheSideWith1lbWeight.extension",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowToTheSideWith1lbWeight.extension:testTimeA4",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowToTheSideWith1lbWeight.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-extended-elbow-to-the-side-with-1lb-weight"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowToTheSideWith1lbWeight.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "透過伸展手肘將重量推向桌子對面的外腕關節"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowToTheSideWith1lbWeight.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aExtendedElbowToTheSideWith1lbWeight.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToTableFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aHandToTableFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToTableFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToTableFront.extension:testTimeA5",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToTableFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-hand-to-table-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToTableFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "將手放在桌上"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToTableFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToTableFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToBoxFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aHandToBoxFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToBoxFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToBoxFront.extension:testTimeA6",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToBoxFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-hand-to-box-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToBoxFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "將手放在桌面上的盒子上"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToBoxFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:aHandToBoxFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:sectionASubscore",
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
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:sectionASubscore.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-timed-joint-segment-movements-subscore"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:sectionASubscore.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "A.定時關節段運動分量表分數"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:sectionASubscore.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedJointSegmentMovements.item:sectionASubscore.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-30",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 30
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "TimedIntegrativeFunctionalMovements",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "B-timed-integrative-functional-movements"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "B.定時整合功能動作評估"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item",
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
        "min" : 10
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bReachAndRetrieveFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bReachAndRetrieveFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bReachAndRetrieveFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bReachAndRetrieveFront.extension:testTimeB1",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bReachAndRetrieveFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-reach-and-retrieve-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bReachAndRetrieveFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "透過手肘和彎曲手腕將 1 磅重的物體拉過桌子"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bReachAndRetrieveFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bReachAndRetrieveFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftCanFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bLiftCanFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftCanFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftCanFront.extension:testTimeB2",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftCanFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-lift-can-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftCanFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "舉起一個罐子，並用圓柱形的抓握方式將其靠近嘴唇"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftCanFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftCanFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftPencilFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bLiftPencilFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftPencilFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftPencilFront.extension:testTimeB3",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftPencilFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-lift-pencil-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftPencilFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "使用三爪卡盤抓握來拿起鉛筆"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftPencilFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftPencilFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bPickUpPaperClipFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bPickUpPaperClipFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bPickUpPaperClipFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bPickUpPaperClipFront.extension:testTimeB4",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bPickUpPaperClipFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-pick-up-paper-clip-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bPickUpPaperClipFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "用鉗子抓取回形針"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bPickUpPaperClipFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bPickUpPaperClipFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bStackCheckersFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bStackCheckersFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bStackCheckersFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bStackCheckersFront.extension:testTimeB5",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeB5",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bStackCheckersFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-stack-checkers-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bStackCheckersFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "將棋子堆疊到中心棋子上"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bStackCheckersFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bStackCheckersFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFlip3CardsFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bFlip3CardsFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFlip3CardsFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFlip3CardsFront.extension:testTimeB6",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeB6",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFlip3CardsFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-flip-3-cards-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFlip3CardsFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "用鉗子抓握，客戶嘗試翻轉每張卡片"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFlip3CardsFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFlip3CardsFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bTurningTheKeyInLockFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bTurningTheKeyInLockFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bTurningTheKeyInLockFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bTurningTheKeyInLockFront.extension:testTimeB7",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeB7",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bTurningTheKeyInLockFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-turning-the-key-in-lock-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bTurningTheKeyInLockFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "使用鉗子抓握並保持接觸，將鑰匙向左和向右旋轉 180 度"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bTurningTheKeyInLockFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bTurningTheKeyInLockFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFoldTowelFront",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bFoldTowelFront",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFoldTowelFront.extension",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFoldTowelFront.extension:testTimeB8",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeB8",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFoldTowelFront.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-fold-towel-front"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFoldTowelFront.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "抓住毛巾，縱向折疊，然後用被測試的手將毛巾再次對折"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFoldTowelFront.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bFoldTowelFront.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftBasketStanding",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bLiftBasketStanding",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftBasketStanding.extension",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftBasketStanding.extension:testTimeB9",
        "path" : "QuestionnaireResponse.item.item.extension",
        "sliceName" : "testTimeB9",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftBasketStanding.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-lift-basket-standing"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftBasketStanding.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "提起一個椅子上 3 磅重的籃子，並將其放在床頭櫃上"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftBasketStanding.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:bLiftBasketStanding.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-5",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:sectionBSubscore",
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
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:sectionBSubscore.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-timed-integrative-functional-movements-subscore"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:sectionBSubscore.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "B.定時關節段運動分量表分數"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:sectionBSubscore.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TimedIntegrativeFunctionalMovements.item:sectionBSubscore.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-45",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 45
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
        "fixedString" : "C-total-score-WMFT"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "C.WMFT總分計算"
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
        "short" : "分數 0-75",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 75
      }
    ]
  }
}

```
