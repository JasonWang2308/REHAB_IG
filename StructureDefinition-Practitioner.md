# Practitioner - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Practitioner**

## Resource Profile: Practitioner 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/Practitioner | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:Practitioner |

 
健康照護服務提供者的標準化定義。 

**Usages:**

* Examples for this Profile: [Practitioner/ot-therapist-001](Practitioner-ot-therapist-001.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/Practitioner)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-Practitioner.csv), [Excel](StructureDefinition-Practitioner.xlsx), [Schematron](StructureDefinition-Practitioner.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "Practitioner",
  "url" : "http://example.org/StructureDefinition/Practitioner",
  "version" : "0.1.0",
  "name" : "Practitioner",
  "title" : "Practitioner",
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
  "description" : "健康照護服務提供者的標準化定義。",
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
  "type" : "Practitioner",
  "baseDefinition" : "https://twcore.mohw.gov.tw/ig/twcore/StructureDefinition/Practitioner-twcore",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Practitioner",
        "path" : "Practitioner"
      },
      {
        "id" : "Practitioner.identifier",
        "path" : "Practitioner.identifier",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "Practitioner.active",
        "path" : "Practitioner.active",
        "min" : 1
      },
      {
        "id" : "Practitioner.name",
        "path" : "Practitioner.name",
        "min" : 1,
        "max" : "1"
      }
    ]
  }
}

```
