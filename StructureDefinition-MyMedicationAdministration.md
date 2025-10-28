# Medication Administration - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Medication Administration**

## Resource Profile: Medication Administration 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/MyMedicationAdministration | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:MyMedicationAdministration |

 
用藥資料 

**Usages:**

* Examples for this Profile: [MedicationAdministration/MyMedicationAdministrationExample](MedicationAdministration-MyMedicationAdministrationExample.md) and [MedicationAdministration/PACMedicationAdministrationExample](MedicationAdministration-PACMedicationAdministrationExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/MyMedicationAdministration)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-MyMedicationAdministration.csv), [Excel](StructureDefinition-MyMedicationAdministration.xlsx), [Schematron](StructureDefinition-MyMedicationAdministration.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "MyMedicationAdministration",
  "url" : "http://example.org/StructureDefinition/MyMedicationAdministration",
  "version" : "0.1.0",
  "name" : "MyMedicationAdministration",
  "title" : "Medication Administration",
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
  "description" : "用藥資料",
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
    },
    {
      "identity" : "w3c.prov",
      "uri" : "http://www.w3.org/ns/prov",
      "name" : "W3C PROV"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "MedicationAdministration",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/MedicationAdministration",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "MedicationAdministration",
        "path" : "MedicationAdministration"
      },
      {
        "id" : "MedicationAdministration.status",
        "path" : "MedicationAdministration.status",
        "short" : "用藥詳細資料",
        "definition" : "欄位用於表達所給予病人的藥物，可以使用CodeableConcept或Reference兩種形式。"
      },
      {
        "id" : "MedicationAdministration.dosage",
        "path" : "MedicationAdministration.dosage",
        "short" : "藥物劑量與給藥方式",
        "definition" : "描述藥物給予的詳細劑量、頻率、途徑等。"
      },
      {
        "id" : "MedicationAdministration.dosage.rate[x]",
        "path" : "MedicationAdministration.dosage.rate[x]",
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
        "id" : "MedicationAdministration.dosage.rate[x]:rateRatio",
        "path" : "MedicationAdministration.dosage.rate[x]",
        "sliceName" : "rateRatio",
        "short" : "藥物輸注速率",
        "definition" : "表示藥物輸注的速度，通常用於輸液，描述單位時間內給予的藥物量。例如每小時100毫升或每分鐘200微克。此欄位以比例(Ratio)方式表達速率，其中分子為用藥量，分母為時間單位。",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Ratio"
          }
        ]
      }
    ]
  }
}

```
