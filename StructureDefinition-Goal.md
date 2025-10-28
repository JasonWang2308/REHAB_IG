# Goal - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Goal**

## Resource Profile: Goal 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/Goal | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:Goal |

 
目標的標準化定義。 

**Usages:**

* Examples for this Profile: [Goal/GoalExample](Goal-GoalExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/Goal)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-Goal.csv), [Excel](StructureDefinition-Goal.xlsx), [Schematron](StructureDefinition-Goal.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "Goal",
  "url" : "http://example.org/StructureDefinition/Goal",
  "version" : "0.1.0",
  "name" : "Goal",
  "title" : "Goal",
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
  "description" : "目標的標準化定義。",
  "fhirVersion" : "4.0.1",
  "mapping" : [
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
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Goal",
  "baseDefinition" : "https://twcore.mohw.gov.tw/ig/twcore/StructureDefinition/Goal-twcore",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Goal",
        "path" : "Goal"
      },
      {
        "id" : "Goal.lifecycleStatus",
        "path" : "Goal.lifecycleStatus",
        "short" : "目標的狀態",
        "definition" : "反映目標目前所處的狀態，例如提案中、執行中、完成、取消等。"
      },
      {
        "id" : "Goal.category",
        "path" : "Goal.category",
        "short" : "目標類型",
        "definition" : "用於分組或分類目標的代碼，例如治療、飲食、行為等。"
      },
      {
        "id" : "Goal.description",
        "path" : "Goal.description",
        "short" : "目標內容說明",
        "definition" : "一段描述此目標的文字或代碼。"
      },
      {
        "id" : "Goal.subject",
        "path" : "Goal.subject",
        "short" : "目標所屬對象",
        "definition" : "此目標所針對的對象，例如病人或特定團體。"
      }
    ]
  }
}

```
