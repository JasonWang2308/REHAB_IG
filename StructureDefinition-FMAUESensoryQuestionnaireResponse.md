# FMAUE感覺評估問卷回覆 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **FMAUE感覺評估問卷回覆**

## Resource Profile: FMAUE感覺評估問卷回覆 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/FMAUESensoryQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:FMAUESensoryQuestionnaireResponse |

 
針對FMAUE上肢感覺評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)
* Examples for this Profile: [QuestionnaireResponse/FMAUESensoryQuestionnaireResponseExample](QuestionnaireResponse-FMAUESensoryQuestionnaireResponseExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/FMAUESensoryQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-FMAUESensoryQuestionnaireResponse.csv), [Excel](StructureDefinition-FMAUESensoryQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-FMAUESensoryQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "FMAUESensoryQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/FMAUESensoryQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "FMAUESensoryQuestionnaireResponse",
  "title" : "FMAUE感覺評估問卷回覆",
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
  "description" : "針對FMAUE上肢感覺評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構",
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
        "fixedCanonical" : "http://example.org/fhir/Questionnaire/FMAUESensoryQuestionnaireInstance"
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
          "description" : "根據linkId區分FMAUE上肢感覺問卷的主要區塊",
          "ordered" : false,
          "rules" : "closed"
        },
        "min" : 7
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "assessmentPhase",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "assessment-phase-fmaue-sensory"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "請選擇評估階段"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "short" : "選項：初評、期中、延展、結案",
        "type" : [
          {
            "code" : "string"
          }
        ]
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
        "fixedString" : "assessment-side-fmaue-sensory"
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
        "id" : "QuestionnaireResponse.item:LightTouch",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "LightTouch",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "A-light-touch"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "A.輕觸覺檢測"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item",
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
        "min" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aUpperArm",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aUpperArm",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aUpperArm.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-upper-arm"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aUpperArm.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "上臂輕觸覺"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aUpperArm.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aUpperArm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aForeArm",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aForeArm",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aForeArm.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-forearm"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aForeArm.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "前臂輕觸覺"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aForeArm.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aForeArm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aHand",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "aHand",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aHand.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "A-I-hand"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aHand.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "手部輕觸覺"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aHand.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:LightTouch.item:aHand.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "Temperature",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "B-temperature"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "B.溫度覺檢測"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item",
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
        "min" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bUpperArm",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bUpperArm",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bUpperArm.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-upper-arm"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bUpperArm.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "上臂溫度覺"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bUpperArm.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bUpperArm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bForeArm",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bForeArm",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bForeArm.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-forearm"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bForeArm.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "前臂溫度覺"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bForeArm.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bForeArm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bHand",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "bHand",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bHand.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "B-I-hand"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bHand.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "手部溫度覺"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bHand.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:Temperature.item:bHand.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "TactileLocalization",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "C-tactile-localization"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "C.觸覺定位檢測"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item",
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
        "min" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cUpperArm",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "cUpperArm",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cUpperArm.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-I-upper-arm"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cUpperArm.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "上臂觸覺定位"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cUpperArm.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cUpperArm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cForeArm",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "cForeArm",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cForeArm.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-I-forearm"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cForeArm.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "前臂觸覺定位"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cForeArm.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cForeArm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cHand",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "cHand",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cHand.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "C-I-hand"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cHand.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "手部觸覺定位"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cHand.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:TactileLocalization.item:cHand.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "PositionSense",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "D-position-sense"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "D.位置覺檢測"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item",
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
        "id" : "QuestionnaireResponse.item:PositionSense.item:dShoulder",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "dShoulder",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dShoulder.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "D-I-shoulder"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dShoulder.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "肩關節位置覺"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dShoulder.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dShoulder.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dElbow",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "dElbow",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dElbow.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "D-I-elbow"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dElbow.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "肘關節位置覺"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dElbow.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dElbow.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dWrist",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "dWrist",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dWrist.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "D-I-wrist"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dWrist.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "腕關節位置覺"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dWrist.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dWrist.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 2
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dThumb",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "dThumb",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ]
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dThumb.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "fixedString" : "D-I-thumb"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dThumb.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "拇指位置覺"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dThumb.answer",
        "path" : "QuestionnaireResponse.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:PositionSense.item:dThumb.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.answer.value[x]",
        "short" : "分數 0-2",
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
        "fixedString" : "E-total-score-FMAUESensory"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "E.FMAUE感覺總分"
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
        "short" : "分數 0-26",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 26
      }
    ]
  }
}

```
