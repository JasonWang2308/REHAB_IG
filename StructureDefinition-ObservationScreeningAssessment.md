# Observation Screening Assessment - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Observation Screening Assessment**

## Resource Profile: Observation Screening Assessment 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/ObservationScreeningAssessment | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:ObservationScreeningAssessment |

 
健康狀態篩檢與評估 

**Usages:**

* Examples for this Profile: [Observation/ObservationScreeningAssessmentExample](Observation-ObservationScreeningAssessmentExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/ObservationScreeningAssessment)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ObservationScreeningAssessment.csv), [Excel](StructureDefinition-ObservationScreeningAssessment.xlsx), [Schematron](StructureDefinition-ObservationScreeningAssessment.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ObservationScreeningAssessment",
  "url" : "http://example.org/StructureDefinition/ObservationScreeningAssessment",
  "version" : "0.1.0",
  "name" : "ObservationScreeningAssessment",
  "title" : "Observation Screening Assessment",
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
  "description" : "健康狀態篩檢與評估",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "workflow",
      "uri" : "http://hl7.org/fhir/workflow",
      "name" : "Workflow Pattern"
    },
    {
      "identity" : "sct-concept",
      "uri" : "http://snomed.info/conceptdomain",
      "name" : "SNOMED CT Concept Domain Binding"
    },
    {
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
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
    },
    {
      "identity" : "sct-attr",
      "uri" : "http://snomed.org/attributebinding",
      "name" : "SNOMED CT Attribute Binding"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Observation",
  "baseDefinition" : "https://twcore.mohw.gov.tw/ig/twcore/StructureDefinition/Observation-screening-assessment-twcore",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Observation",
        "path" : "Observation"
      },
      {
        "id" : "Observation.status",
        "path" : "Observation.status",
        "short" : "觀察結果狀態",
        "definition" : "觀察結果的當前狀態，例如完成、暫停或取消。"
      },
      {
        "id" : "Observation.category",
        "path" : "Observation.category",
        "short" : "觀察類別",
        "definition" : "觀察結果所屬分類，例如篩檢評估，方便分類整理。"
      },
      {
        "id" : "Observation.code",
        "path" : "Observation.code",
        "short" : "觀察測量項目",
        "definition" : "觀察的具體評估項目或篩檢指標的代碼與名稱。"
      },
      {
        "id" : "Observation.subject",
        "path" : "Observation.subject",
        "short" : "受測者",
        "definition" : "本次觀察所針對的病患或個案。"
      },
      {
        "id" : "Observation.effective[x]",
        "path" : "Observation.effective[x]",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "type",
              "path" : "$this"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        }
      },
      {
        "id" : "Observation.effective[x]:effectiveDateTime",
        "path" : "Observation.effective[x]",
        "sliceName" : "effectiveDateTime",
        "short" : "觀察時間",
        "definition" : "觀察或評估實施的時間。",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-type-must-support",
                "valueBoolean" : true
              }
            ],
            "code" : "dateTime"
          }
        ]
      },
      {
        "id" : "Observation.value[x]",
        "path" : "Observation.value[x]",
        "short" : "觀察值",
        "definition" : "觀察或評估的結果值，可能為數字、文字或其他類型資料。"
      },
      {
        "id" : "Observation.interpretation",
        "path" : "Observation.interpretation",
        "short" : "結果判讀",
        "definition" : "對觀察結果的解讀或評估，例如正常或異常。"
      },
      {
        "id" : "Observation.note",
        "path" : "Observation.note",
        "short" : "備註",
        "definition" : "補充說明或相關註記資訊。"
      }
    ]
  }
}

```
