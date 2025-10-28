# MRCQuestionnaireResponse - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MRCQuestionnaireResponse**

## Resource Profile: MRCQuestionnaireResponse 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/MRCQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:MRCQuestionnaireResponse |

 
MRC問卷回覆 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/MRCQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-MRCQuestionnaireResponse.csv), [Excel](StructureDefinition-MRCQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-MRCQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "MRCQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/MRCQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "MRCQuestionnaireResponse",
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
  "description" : "MRC問卷回覆",
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
        "patternCanonical" : "http://example.org/Questionnaire/MRCQuestionnaireInstance"
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
        "min" : 3
      },
      {
        "id" : "QuestionnaireResponse.item:abduction-arm",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "abduction-arm",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:abduction-arm.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:abduction-arm.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:abduction-arm.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "abduction-arm"
      },
      {
        "id" : "QuestionnaireResponse.item:abduction-arm.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "肩關節外展"
      },
      {
        "id" : "QuestionnaireResponse.item:abduction-arm.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:abduction-arm.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:abduction-arm.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:abduction-arm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:flexion-forearm",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "flexion-forearm",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:flexion-forearm.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:flexion-forearm.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:flexion-forearm.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "flexion-forearm"
      },
      {
        "id" : "QuestionnaireResponse.item:flexion-forearm.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "前臂屈曲"
      },
      {
        "id" : "QuestionnaireResponse.item:flexion-forearm.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:flexion-forearm.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:flexion-forearm.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:flexion-forearm.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      },
      {
        "id" : "QuestionnaireResponse.item:extension-wrist",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "extension-wrist",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:extension-wrist.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:extension-wrist.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:extension-wrist.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "extension-wrist"
      },
      {
        "id" : "QuestionnaireResponse.item:extension-wrist.text",
        "path" : "QuestionnaireResponse.item.text",
        "patternString" : "手腕向上伸張"
      },
      {
        "id" : "QuestionnaireResponse.item:extension-wrist.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item:extension-wrist.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:extension-wrist.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:extension-wrist.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "integer"
          }
        ],
        "minValueInteger" : 0,
        "maxValueInteger" : 5
      }
    ]
  }
}

```
