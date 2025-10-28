# Organization - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Organization**

## Resource Profile: Organization 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/Organization | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:Organization |

 
機構的標準化定義。 

**Usages:**

* Examples for this Profile: [台灣健康醫院](Organization-OrganizationExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/Organization)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-Organization.csv), [Excel](StructureDefinition-Organization.xlsx), [Schematron](StructureDefinition-Organization.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "Organization",
  "url" : "http://example.org/StructureDefinition/Organization",
  "version" : "0.1.0",
  "name" : "Organization",
  "title" : "Organization",
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
  "description" : "機構的標準化定義。",
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
      "identity" : "servd",
      "uri" : "http://www.omg.org/spec/ServD/1.0/",
      "name" : "ServD"
    },
    {
      "identity" : "w5",
      "uri" : "http://hl7.org/fhir/fivews",
      "name" : "FiveWs Pattern Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Organization",
  "baseDefinition" : "https://twcore.mohw.gov.tw/ig/twcore/StructureDefinition/Organization-twcore",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Organization",
        "path" : "Organization"
      },
      {
        "id" : "Organization.identifier",
        "path" : "Organization.identifier",
        "short" : "機構識別碼",
        "definition" : "跨多個系統中識別此機構的唯一編號。",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "Organization.active",
        "path" : "Organization.active",
        "short" : "是否啟用",
        "definition" : "此機構的紀錄是否仍在使用中。",
        "min" : 1
      },
      {
        "id" : "Organization.name",
        "path" : "Organization.name",
        "short" : "機構名稱",
        "definition" : "機構使用的正式名稱。",
        "min" : 1
      },
      {
        "id" : "Organization.address",
        "path" : "Organization.address",
        "short" : "機構地址",
        "definition" : "機構的實體地址，包含縣市、區域、街道等資訊。",
        "min" : 1,
        "max" : "1"
      }
    ]
  }
}

```
