# FMAUE動作評估問卷回覆 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **FMAUE動作評估問卷回覆**

## Resource Profile: FMAUE動作評估問卷回覆 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/FMAUEMotionQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:FMAUEMotionQuestionnaireResponse |

 
針對FMAUE上肢動作評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/FMAUEMotionQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-FMAUEMotionQuestionnaireResponse.csv), [Excel](StructureDefinition-FMAUEMotionQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-FMAUEMotionQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "FMAUEMotionQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/FMAUEMotionQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "FMAUEMotionQuestionnaireResponse",
  "title" : "FMAUE動作評估問卷回覆",
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
  "description" : "針對FMAUE上肢動作評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構",
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
        "fixedCanonical" : "http://example.org/fhir/Questionnaire/FMAUEMotorQuestionnaireInstance"
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
          "description" : "根據LinkId區分FMAUE上肢感覺問卷的主要區塊",
          "ordered" : false,
          "rules" : "closed"
        },
        "min" : 6
      },
      {
        "id" : "QuestionnaireResponse.item:assessmentPhase",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "assessmentPhase",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
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
        "fixedString" : "assessment-phase-fmaue-motion"
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
        "fixedString" : "assessment-side-fmaue-motion"
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "ShoulderElbowForearm",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "A-shoulder-elbow-forearm"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "A.肩部/肘部/前臂"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item",
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
        "min" : 6
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "a1",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "A-I-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "I.反射反應"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item",
        "path" : "QuestionnaireResponse.item.item.item",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Flexors",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Flexors",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Flexors.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-I-a-flexors"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Flexors.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "二頭肌或手指屈肌"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Flexors.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Flexors.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Extensors",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Extensors",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Extensors.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-I-a-extensors"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Extensors.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "三頭肌"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Extensors.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a1.item:Extensors.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "a2a",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "A-II-a-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "II.a.屈肌協同動作"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item",
        "path" : "QuestionnaireResponse.item.item.item",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "linkId"
            }
          ],
          "rules" : "closed"
        },
        "min" : 6
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderRetraction",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ShoulderRetraction",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderRetraction.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-II-a-shoulder-retraction"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderRetraction.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "肩部回縮"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderRetraction.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderRetraction.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderElevation",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ShoulderElevation",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderElevation.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-II-a-shoulder-elevation"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderElevation.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "肩部抬高"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderElevation.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderElevation.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderAbduction",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ShoulderAbduction",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderAbduction.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-II-a-shoulder-abduction"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderAbduction.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "肩外展"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderAbduction.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderAbduction.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderOutwardsRotation",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ShoulderOutwardsRotation",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderOutwardsRotation.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-II-a-shoulder-outwards-rotation"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderOutwardsRotation.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "肩膀外旋"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderOutwardsRotation.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ShoulderOutwardsRotation.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
        "short" : "分數 0-2",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 0
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ElbowFlexion",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ElbowFlexion",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ElbowFlexion.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-II-a-elbow-flexion"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ElbowFlexion.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手肘屈曲"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ElbowFlexion.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ElbowFlexion.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ForearmSupination",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ForearmSupination",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ForearmSupination.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-II-a-forearm-supination"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ForearmSupination.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "前臂旋後"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ForearmSupination.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2a.item:ForearmSupination.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "a2b",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "A-II-b-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "II.b.伸肌協同動作"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item",
        "path" : "QuestionnaireResponse.item.item.item",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ShoulderAddInwardRotation",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ShoulderAddInwardRotation",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ShoulderAddInwardRotation.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-II-b-shoulder-add-inward-rotation"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ShoulderAddInwardRotation.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "肩部內旋/外旋"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ShoulderAddInwardRotation.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ShoulderAddInwardRotation.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ElbowExtension",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ElbowExtension",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ElbowExtension.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-II-b-elbow-extension"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ElbowExtension.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手肘伸展"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ElbowExtension.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ElbowExtension.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ForearmPronation",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ForearmPronation",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ForearmPronation.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-II-b-forearm-pronation"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ForearmPronation.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "前臂旋前"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ForearmPronation.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a2b.item:ForearmPronation.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "a3",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "A-III-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "III.部份協同動作（不可代償）"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item",
        "path" : "QuestionnaireResponse.item.item.item",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:HandToLumbarSpine",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "HandToLumbarSpine",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:HandToLumbarSpine.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-III-hand-to-lumbar-spine"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:HandToLumbarSpine.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手到腰椎"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:HandToLumbarSpine.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:HandToLumbarSpine.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ShoulderFlexion090",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ShoulderFlexion090",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ShoulderFlexion090.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-III-shoulder-flexion-0-90"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ShoulderFlexion090.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "肩部屈曲0° - 90°"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ShoulderFlexion090.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ShoulderFlexion090.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ElbowProSupination",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ElbowProSupination",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ElbowProSupination.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-III-elbow-pro-supination"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ElbowProSupination.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手肘 90° 前傾/旋後"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ElbowProSupination.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a3.item:ElbowProSupination.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "a4",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "A-IV-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "IV.自主運動"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item",
        "path" : "QuestionnaireResponse.item.item.item",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderAbduction090",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ShoulderAbduction090",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderAbduction090.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-IV-shoulder-abduction-0-90"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderAbduction090.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "肩外展 0° - 90°"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderAbduction090.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderAbduction090.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderFlexion90180",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ShoulderFlexion90180",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderFlexion90180.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-IV-shoulder-flexion-90-180"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderFlexion90180.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手肘 90° 前傾/旋後"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderFlexion90180.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ShoulderFlexion90180.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ElbowProSupination",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "ElbowProSupination",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ElbowProSupination.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-IV-elbow-0-pronation-supination"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ElbowProSupination.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手肘 0° 前傾/旋後"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ElbowProSupination.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a4.item:ElbowProSupination.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a5",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "a5",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a5.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "A-V-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a5.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "V.反射強度"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a5.item",
        "path" : "QuestionnaireResponse.item.item.item",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "linkId"
            }
          ],
          "rules" : "closed"
        },
        "min" : 1
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a5.item:NormalReflexActivity",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "NormalReflexActivity",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a5.item:NormalReflexActivity.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "A-V-normal-reflex-activity"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a5.item:NormalReflexActivity.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "正常反射活動（屈肌/伸肌）"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a5.item:NormalReflexActivity.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:ShoulderElbowForearm.item:a5.item:NormalReflexActivity.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "WristHand",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "B-wrist-hand"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "B.手腕/手部"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b1",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "b1",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "B-I-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "I.手腕穩定度"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item",
        "path" : "QuestionnaireResponse.item.item.item",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristStability",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Elbow90WristStability",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristStability.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-I-elbow-90-wrist-stability"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristStability.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手肘 90° 腕部穩定性"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristStability.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristStability.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristFlexExtension",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Elbow90WristFlexExtension",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristFlexExtension.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-I-elbow-90-wrist-flex-extension"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristFlexExtension.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手肘 90° 腕關節屈曲/伸展"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristFlexExtension.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow90WristFlexExtension.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristStability",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Elbow0WristStability",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristStability.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-I-elbow-0-wrist-stability"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristStability.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手肘 0° 腕部穩定性"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristStability.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristStability.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristFlexExtension",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Elbow0WristFlexExtension",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristFlexExtension.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-I-elbow-0-wrist-flex-extension"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristFlexExtension.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手肘 0° 腕部屈曲/伸展"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristFlexExtension.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:Elbow0WristFlexExtension.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:WristCircumduction",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "WristCircumduction",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:WristCircumduction.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-I-wrist-circumduction"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:WristCircumduction.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "腕部旋轉"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:WristCircumduction.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b1.item:WristCircumduction.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b2",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "b2",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "B-II-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "II.手指伸屈"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item",
        "path" : "QuestionnaireResponse.item.item.item",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassFlexion",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "FingersMassFlexion",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassFlexion.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-II-fingers-mass-flexion"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassFlexion.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手指屈曲"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassFlexion.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassFlexion.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassExtension",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "FingersMassExtension",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassExtension.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-II-fingers-mass-extension"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassExtension.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手指伸展"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassExtension.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b2.item:FingersMassExtension.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b3",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "b3",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "B-III-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "III.抓握功能"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item",
        "path" : "QuestionnaireResponse.item.item.item",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_a",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Grasp_a",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_a.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-III-grasp-a"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_a.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "a. MP 關節伸展，PIP 和 DIP 彎曲；測試抓握力是否抵抗阻力"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_a.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_a.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_b",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Grasp_b",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_b.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-III-grasp-b"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_b.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "b. 指導患者將拇指內收，其他關節在 0° 位置"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_b.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_b.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_c",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Grasp_c",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_c.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-III-grasp-c"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_c.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "c. 食指拇指肚對著，中間插一支鉛筆"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_c.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_c.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_d",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Grasp_d",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_d.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-III-grasp-d"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_d.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "d. 患者用食指和中指的掌側表面互相抵住，抓住一個圓柱形物體（小罐子）。"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_d.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_d.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_e",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Grasp_e",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_e.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "B-III-grasp-e"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_e.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "e. 球形抓握；病人抓住一個網球"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_e.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:WristHand.item:b3.item:Grasp_e.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:CoordinationSpeed",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "CoordinationSpeed",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "patternString" : "C-coordination-speed"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "C.協調性/速度"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item",
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
        "min" : 1
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1",
        "path" : "QuestionnaireResponse.item.item",
        "sliceName" : "c1",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.linkId",
        "path" : "QuestionnaireResponse.item.item.linkId",
        "patternString" : "C-I-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.text",
        "path" : "QuestionnaireResponse.item.item.text",
        "patternString" : "I.協調性/速度"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item",
        "path" : "QuestionnaireResponse.item.item.item",
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
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Tremor",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Tremor",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Tremor.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "C-I-finger-to-nose-tremor"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Tremor.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手指觸碰鼻子：顫抖"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Tremor.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Tremor.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Dysmetria",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Dysmetria",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Dysmetria.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "C-I-finger-to-nose-dysmetria"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Dysmetria.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手指觸鼻：辨距不良"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Dysmetria.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Dysmetria.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Time",
        "path" : "QuestionnaireResponse.item.item.item",
        "sliceName" : "Time",
        "min" : 1,
        "max" : "1",
        "type" : [
          {
            "code" : "BackboneElement"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Time.linkId",
        "path" : "QuestionnaireResponse.item.item.item.linkId",
        "fixedString" : "C-I-finger-to-nose-time"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Time.text",
        "path" : "QuestionnaireResponse.item.item.item.text",
        "patternString" : "手指到鼻子：時間"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Time.answer",
        "path" : "QuestionnaireResponse.item.item.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:CoordinationSpeed.item:c1.item:Time.answer.value[x]",
        "path" : "QuestionnaireResponse.item.item.item.answer.value[x]",
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
        "fixedString" : "D-total-score-FMAUEMotion"
      },
      {
        "id" : "QuestionnaireResponse.item:totalScoreSection.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "D.FMAUE動作總分"
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
        "short" : "分數 0-66",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 66
      }
    ]
  }
}

```
