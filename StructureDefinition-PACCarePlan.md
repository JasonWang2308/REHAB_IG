# PACCarePlan - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PACCarePlan**

## Resource Profile: PACCarePlan 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/PACCarePlan | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:PACCarePlan |

 
PAC照護計畫的標準化定義的內容 

**Usages:**

* Examples for this Profile: [CarePlan/PACCarePlanExample](CarePlan-PACCarePlanExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/PACCarePlan)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-PACCarePlan.csv), [Excel](StructureDefinition-PACCarePlan.xlsx), [Schematron](StructureDefinition-PACCarePlan.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "PACCarePlan",
  "url" : "http://example.org/StructureDefinition/PACCarePlan",
  "version" : "0.1.0",
  "name" : "PACCarePlan",
  "title" : "PACCarePlan",
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
  "description" : "PAC照護計畫的標準化定義的內容",
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
      }
    ]
  }
}

```
