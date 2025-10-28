# PACCondition - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PACCondition**

## Resource Profile: PACCondition 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/PACCondition | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:PACCondition |

 
進行患者上肢功能評估時的狀況資訊，應包含待評估身體部位或病徵。 

**Usages:**

* Use this Profile: [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/PACCondition)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-PACCondition.csv), [Excel](StructureDefinition-PACCondition.xlsx), [Schematron](StructureDefinition-PACCondition.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "PACCondition",
  "url" : "http://example.org/StructureDefinition/PACCondition",
  "version" : "0.1.0",
  "name" : "PACCondition",
  "title" : "PACCondition",
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
  "description" : "進行患者上肢功能評估時的狀況資訊，應包含待評估身體部位或病徵。",
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
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Condition",
  "baseDefinition" : "https://twcore.mohw.gov.tw/ig/twcore/StructureDefinition/Condition-twcore",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Condition",
        "path" : "Condition"
      },
      {
        "id" : "Condition.category",
        "path" : "Condition.category",
        "patternCodeableConcept" : {
          "coding" : [
            {
              "system" : "http://terminology.hl7.org/CodeSystem/condition-category",
              "code" : "encounter-diagnosis"
            }
          ]
        }
      },
      {
        "id" : "Condition.bodySite",
        "path" : "Condition.bodySite",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "linkId"
            }
          ],
          "description" : "依據需求填入評估部位或是實際患部/側，至少應填入評估部位",
          "ordered" : true,
          "rules" : "closed"
        },
        "min" : 1
      },
      {
        "id" : "Condition.bodySite:AssessmentSite",
        "path" : "Condition.bodySite",
        "sliceName" : "AssessmentSite",
        "min" : 1,
        "max" : "*",
        "mustSupport" : true
      },
      {
        "id" : "Condition.bodySite:AffectedPart",
        "path" : "Condition.bodySite",
        "sliceName" : "AffectedPart",
        "min" : 0,
        "max" : "*",
        "mustSupport" : true
      }
    ]
  }
}

```
