# 評估問卷 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **評估問卷**

## Resource Profile: 評估問卷 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/SPACQuestionnaire | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:SPACQuestionnaire |

 
評估問卷的結構化定義，實際問卷內容請參考Structure: Questionnaire，可依據前者內容做為範本進行擴充 

**Usages:**

* Examples for this Profile: [ARATQuestionnaire](Questionnaire-ARATQuestionnaireInstance.md), [Questionnaire/BarthelQuestionnaireInstance](Questionnaire-BarthelQuestionnaireInstance.md), [FMAUEMotorQuestionnaire](Questionnaire-FMAUEMotorQuestionnaireInstance.md), [FMAUESensoryQuestionnaire](Questionnaire-FMAUESensoryQuestionnaireInstance.md)...Show 5 more,[IDALQuestionnaireInstance](Questionnaire-IDALQuestionnaireInstance.md),[Questionnaire/MASQuestionnaireInstance](Questionnaire-MASQuestionnaireInstance.md),[Questionnaire/MMSEQuestionnaireInstance](Questionnaire-MMSEQuestionnaireInstance.md),[Questionnaire/MRCQuestionnaireInstance](Questionnaire-MRCQuestionnaireInstance.md)and[WMFTQuestionnaire](Questionnaire-WMFTQuestionnaireInstance.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/SPACQuestionnaire)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-SPACQuestionnaire.csv), [Excel](StructureDefinition-SPACQuestionnaire.xlsx), [Schematron](StructureDefinition-SPACQuestionnaire.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "SPACQuestionnaire",
  "url" : "http://example.org/StructureDefinition/SPACQuestionnaire",
  "version" : "0.1.0",
  "name" : "SPACQuestionnaire",
  "title" : "評估問卷",
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
  "description" : "評估問卷的結構化定義，實際問卷內容請參考Structure: Questionnaire，可依據前者內容做為範本進行擴充",
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
      "identity" : "objimpl",
      "uri" : "http://hl7.org/fhir/object-implementation",
      "name" : "Object Implementation Information"
    },
    {
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Questionnaire",
  "baseDefinition" : "http://hl7.org/fhir/uv/sdc/StructureDefinition/sdc-questionnaire-extr-obsn",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Questionnaire",
        "path" : "Questionnaire"
      },
      {
        "id" : "Questionnaire.identifier",
        "path" : "Questionnaire.identifier",
        "mustSupport" : true
      },
      {
        "id" : "Questionnaire.name",
        "path" : "Questionnaire.name",
        "mustSupport" : true
      },
      {
        "id" : "Questionnaire.description",
        "path" : "Questionnaire.description",
        "mustSupport" : true
      },
      {
        "id" : "Questionnaire.item",
        "path" : "Questionnaire.item",
        "min" : 1
      }
    ]
  }
}

```
