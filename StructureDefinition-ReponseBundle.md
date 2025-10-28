# Bundle-評估資料回傳 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Bundle-評估資料回傳**

## Resource Profile: Bundle-評估資料回傳 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/ReponseBundle | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:ReponseBundle |

 
此 Profile 定義了上肢功能評估資料須包含的資訊。 

**Usages:**

* This Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/ReponseBundle)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ReponseBundle.csv), [Excel](StructureDefinition-ReponseBundle.xlsx), [Schematron](StructureDefinition-ReponseBundle.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ReponseBundle",
  "url" : "http://example.org/StructureDefinition/ReponseBundle",
  "version" : "0.1.0",
  "name" : "ReponseBundle",
  "title" : "Bundle-評估資料回傳",
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
  "description" : "此 Profile 定義了上肢功能評估資料須包含的資訊。",
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
      "identity" : "cda",
      "uri" : "http://hl7.org/v3/cda",
      "name" : "CDA (R2)"
    },
    {
      "identity" : "w5",
      "uri" : "http://hl7.org/fhir/fivews",
      "name" : "FiveWs Pattern Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Bundle",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Bundle",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Bundle",
        "path" : "Bundle"
      },
      {
        "id" : "Bundle.type",
        "path" : "Bundle.type",
        "short" : "Bundle的類型",
        "patternCode" : "transaction",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry",
        "path" : "Bundle.entry",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "profile",
              "path" : "resource"
            }
          ],
          "rules" : "open"
        },
        "min" : 15,
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Patient",
        "path" : "Bundle.entry",
        "sliceName" : "Patient",
        "short" : "患者基本資料",
        "min" : 1,
        "max" : "*",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Patient.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Patient"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Condition",
        "path" : "Bundle.entry",
        "sliceName" : "Condition",
        "short" : "患者評估狀況",
        "min" : 1,
        "max" : "*",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Condition.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Condition",
            "profile" : ["http://example.org/StructureDefinition/PACCondition"]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Organization",
        "path" : "Bundle.entry",
        "sliceName" : "Organization",
        "short" : "進行評估機構",
        "min" : 0,
        "max" : "*",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Organization.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Organization"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Practitioner",
        "path" : "Bundle.entry",
        "sliceName" : "Practitioner",
        "short" : "評估者",
        "min" : 1,
        "max" : "*",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Practitioner.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Practitioner"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Practitioner-Role",
        "path" : "Bundle.entry",
        "sliceName" : "Practitioner-Role",
        "short" : "評估者身分",
        "min" : 0,
        "max" : "*",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:Practitioner-Role.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "PractitionerRole"
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-FMAUE-Motion",
        "path" : "Bundle.entry",
        "sliceName" : "QR-FMAUE-Motion",
        "short" : "Fugl-Meyer上肢動作評估",
        "min" : 0,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-FMAUE-Motion.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/FMAUEMotionQuestionnaireResponse"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-FMAUE-Sensory",
        "path" : "Bundle.entry",
        "sliceName" : "QR-FMAUE-Sensory",
        "short" : "Fugl-Meyer上肢感覺評估",
        "min" : 0,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-FMAUE-Sensory.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/FMAUESensoryQuestionnaireResponse"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-ARAT",
        "path" : "Bundle.entry",
        "sliceName" : "QR-ARAT",
        "short" : "ARAT評估",
        "min" : 0,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-ARAT.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/ARATQuestionnaireResponse"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-WMFT",
        "path" : "Bundle.entry",
        "sliceName" : "QR-WMFT",
        "short" : "WMFT評估",
        "min" : 0,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-WMFT.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/WMFTQuestionnaireResponse"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-IADL",
        "path" : "Bundle.entry",
        "sliceName" : "QR-IADL",
        "short" : "IADL評估",
        "min" : 0,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-IADL.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/IADLQuestionnaireResponse"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-MAS",
        "path" : "Bundle.entry",
        "sliceName" : "QR-MAS",
        "short" : "MAS評估",
        "min" : 0,
        "max" : "*",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-MAS.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/MASQuestionnaireResponse"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-MRC",
        "path" : "Bundle.entry",
        "sliceName" : "QR-MRC",
        "short" : "MRC評估",
        "min" : 0,
        "max" : "*",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-MRC.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/MRCQuestionnaireResponse"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-MMSE",
        "path" : "Bundle.entry",
        "sliceName" : "QR-MMSE",
        "short" : "MMSE評估",
        "min" : 0,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-MMSE.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/MMSEQuestionnaireResponse"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-Barthel",
        "path" : "Bundle.entry",
        "sliceName" : "QR-Barthel",
        "short" : "Barthel評估",
        "min" : 0,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-Barthel.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/BarthelQuestionnaireResponse"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-BBT",
        "path" : "Bundle.entry",
        "sliceName" : "QR-BBT",
        "short" : "BBT評估",
        "min" : 0,
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Bundle.entry:QR-BBT.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "QuestionnaireResponse",
            "profile" : [
              "http://example.org/StructureDefinition/bbt-questionnaire-response"
            ]
          }
        ],
        "mustSupport" : true
      }
    ]
  }
}

```
