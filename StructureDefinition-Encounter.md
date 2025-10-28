# Encounter - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Encounter**

## Resource Profile: Encounter 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/Encounter | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:Encounter |

 
就醫事件的標準化定義。 

**Usages:**

* Examples for this Profile: [Encounter/arat-assessment-encounter-001](Encounter-arat-assessment-encounter-001.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/Encounter)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-Encounter.csv), [Excel](StructureDefinition-Encounter.xlsx), [Schematron](StructureDefinition-Encounter.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "Encounter",
  "url" : "http://example.org/StructureDefinition/Encounter",
  "version" : "0.1.0",
  "name" : "Encounter",
  "title" : "Encounter",
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
  "description" : "就醫事件的標準化定義。",
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
  "type" : "Encounter",
  "baseDefinition" : "https://twcore.mohw.gov.tw/ig/twcore/StructureDefinition/Encounter-twcore",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Encounter",
        "path" : "Encounter"
      },
      {
        "id" : "Encounter.status",
        "path" : "Encounter.status",
        "short" : "狀態代碼，表示就醫事件的流轉狀態",
        "definition" : "此欄位表示該就醫事件是否處於啟用、草稿、完成等狀態；必填。"
      },
      {
        "id" : "Encounter.subject",
        "path" : "Encounter.subject",
        "min" : 1
      },
      {
        "id" : "Encounter.period",
        "path" : "Encounter.period",
        "definition" : "就醫的開始和結束時間。如果（尚）不知道，可以省略「期間」裡的結束日期時間。",
        "min" : 1
      }
    ]
  }
}

```
