# PractitionerRole - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PractitionerRole**

## Resource Profile: PractitionerRole 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/PractitionerRole | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:PractitionerRole |

 
健康照護服務提供者角色的標準化定義。 

**Usages:**

* Examples for this Profile: [PractitionerRole/PractitionerRoleExample](PractitionerRole-PractitionerRoleExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/PractitionerRole)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-PractitionerRole.csv), [Excel](StructureDefinition-PractitionerRole.xlsx), [Schematron](StructureDefinition-PractitionerRole.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "PractitionerRole",
  "url" : "http://example.org/StructureDefinition/PractitionerRole",
  "version" : "0.1.0",
  "name" : "PractitionerRole",
  "title" : "PractitionerRole",
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
  "description" : "健康照護服務提供者角色的標準化定義。",
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
  "type" : "PractitionerRole",
  "baseDefinition" : "https://twcore.mohw.gov.tw/ig/twcore/StructureDefinition/PractitionerRole-twcore",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "PractitionerRole",
        "path" : "PractitionerRole"
      },
      {
        "id" : "PractitionerRole.active",
        "path" : "PractitionerRole.active",
        "min" : 1
      },
      {
        "id" : "PractitionerRole.practitioner",
        "path" : "PractitionerRole.practitioner",
        "min" : 1
      },
      {
        "id" : "PractitionerRole.organization",
        "path" : "PractitionerRole.organization",
        "min" : 1
      },
      {
        "id" : "PractitionerRole.code",
        "path" : "PractitionerRole.code",
        "min" : 1,
        "max" : "1"
      }
    ]
  }
}

```
