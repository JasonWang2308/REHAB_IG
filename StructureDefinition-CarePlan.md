# Care Plan - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Care Plan**

## Resource Profile: Care Plan 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/CarePlan | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:CarePlan |

 
照護計畫 

**Usages:**

* Examples for this Profile: [CarePlan/CarePlanExample](CarePlan-CarePlanExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/CarePlan)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-CarePlan.csv), [Excel](StructureDefinition-CarePlan.xlsx), [Schematron](StructureDefinition-CarePlan.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "CarePlan",
  "url" : "http://example.org/StructureDefinition/CarePlan",
  "version" : "0.1.0",
  "name" : "CarePlan",
  "title" : "Care Plan",
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
  "description" : "照護計畫",
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
    },
    {
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "CarePlan",
  "baseDefinition" : "https://twcore.mohw.gov.tw/ig/twcore/StructureDefinition/CarePlan-twcore",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "CarePlan",
        "path" : "CarePlan"
      },
      {
        "id" : "CarePlan.status",
        "path" : "CarePlan.status",
        "short" : "狀態代碼，表示照護計畫的流轉狀態",
        "definition" : "此欄位表示該照護計畫是否處於啟用、草稿、完成等狀態；必填。"
      },
      {
        "id" : "CarePlan.intent",
        "path" : "CarePlan.intent",
        "short" : "照護計畫的執行意圖 (如提案, 規劃, 指令, 選項)",
        "definition" : "標示這個照護計劃現在是提案、正式計畫、指令還是僅供參考的選項。"
      },
      {
        "id" : "CarePlan.category",
        "path" : "CarePlan.category",
        "definition" : "計畫的類型，例如：營養及飲食指導、惡化徵兆偵測及必要處理等。"
      },
      {
        "id" : "CarePlan.description",
        "path" : "CarePlan.description",
        "short" : "計畫摘要說明",
        "definition" : "本欄位用於簡要描述照護計畫的性質與目標，提供整體計畫的概要說明。"
      },
      {
        "id" : "CarePlan.subject",
        "path" : "CarePlan.subject",
        "definition" : "指向台灣機器手訓練 Patient 資源，用於標記本照護計畫所屬的病患或病患群體。",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : ["http://example.org/StructureDefinition/Patient"]
          }
        ]
      }
    ]
  }
}

```
