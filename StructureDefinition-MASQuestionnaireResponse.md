# MAS 量表問卷回覆 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MAS 量表問卷回覆**

## Resource Profile: MAS 量表問卷回覆 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/MASQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:MASQuestionnaireResponse |

 
Modified Ashworth Scale (MAS) 評估量表問卷回覆 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)
* Examples for this Profile: [QuestionnaireResponse/MASQuestionnaireResponseExample](QuestionnaireResponse-MASQuestionnaireResponseExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/MASQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-MASQuestionnaireResponse.csv), [Excel](StructureDefinition-MASQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-MASQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "MASQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/MASQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "MASQuestionnaireResponse",
  "title" : "MAS 量表問卷回覆",
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
  "description" : "Modified Ashworth Scale (MAS) 評估量表問卷回覆",
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
        "patternCanonical" : "http://example.org/Questionnaire/MASQuestionnaireInstance"
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
        "min" : 6
      },
      {
        "id" : "QuestionnaireResponse.item.answer",
        "path" : "QuestionnaireResponse.item.answer",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "QuestionnaireResponse.item.answer.value[x]",
        "path" : "QuestionnaireResponse.item.answer.value[x]",
        "type" : [
          {
            "code" : "Coding"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://example.org/ValueSet/mas-score"
        }
      },
      {
        "id" : "QuestionnaireResponse.item:left-shoulder",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "left-shoulder",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:left-shoulder.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:left-shoulder.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:left-shoulder.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "left-shoulder"
      },
      {
        "id" : "QuestionnaireResponse.item:left-shoulder.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:left-shoulder.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:left-wrist",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "left-wrist",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:left-wrist.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:left-wrist.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:left-wrist.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "left-wrist"
      },
      {
        "id" : "QuestionnaireResponse.item:left-wrist.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:left-wrist.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
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
        "id" : "QuestionnaireResponse.item:left-hand.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:left-hand.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:left-hand.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "left-hand"
      },
      {
        "id" : "QuestionnaireResponse.item:left-hand.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:left-hand.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:right-shoulder",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "right-shoulder",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:right-shoulder.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:right-shoulder.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:right-shoulder.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "right-shoulder"
      },
      {
        "id" : "QuestionnaireResponse.item:right-shoulder.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:right-shoulder.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      },
      {
        "id" : "QuestionnaireResponse.item:right-wrist",
        "path" : "QuestionnaireResponse.item",
        "sliceName" : "right-wrist",
        "min" : 1,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item:right-wrist.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:right-wrist.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:right-wrist.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "right-wrist"
      },
      {
        "id" : "QuestionnaireResponse.item:right-wrist.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:right-wrist.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
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
        "id" : "QuestionnaireResponse.item:right-hand.extension:itemMedia",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "itemMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:right-hand.extension:ItemSignature",
        "path" : "QuestionnaireResponse.item.extension",
        "sliceName" : "ItemSignature"
      },
      {
        "id" : "QuestionnaireResponse.item:right-hand.linkId",
        "path" : "QuestionnaireResponse.item.linkId",
        "fixedString" : "right-hand"
      },
      {
        "id" : "QuestionnaireResponse.item:right-hand.answer.extension:itemAnswerMedia",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "itemAnswerMedia"
      },
      {
        "id" : "QuestionnaireResponse.item:right-hand.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue"
      }
    ]
  }
}

```
