# Patient - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Patient**

## Resource Profile: Patient 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/Patient | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:Patient |

 
病人的資料定義範例，包含姓名、識別碼等基本資訊 

**Usages:**

* Refer to this Profile: [ARAT上肢功能評估問卷回覆](StructureDefinition-ARATQuestionnaireResponse.md), [Care Plan](StructureDefinition-CarePlan.md), [FMAUE動作評估問卷回覆](StructureDefinition-FMAUEMotionQuestionnaireResponse.md), [FMAUE感覺評估問卷回覆](StructureDefinition-FMAUESensoryQuestionnaireResponse.md)...Show 3 more,[IADL評估問卷回覆](StructureDefinition-IADLQuestionnaireResponse.md),[MMSE QuestionnaireResponse (scored)](StructureDefinition-MMSEQuestionnaireResponse.md)and[WMFT上肢功能評估問卷回覆](StructureDefinition-WMFTQuestionnaireResponse.md)
* Examples for this Profile: [Patient/stroke-patient-001](Patient-stroke-patient-001.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/Patient)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-Patient.csv), [Excel](StructureDefinition-Patient.xlsx), [Schematron](StructureDefinition-Patient.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "Patient",
  "url" : "http://example.org/StructureDefinition/Patient",
  "version" : "0.1.0",
  "name" : "Patient",
  "title" : "Patient",
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
  "description" : "病人的資料定義範例，包含姓名、識別碼等基本資訊",
  "fhirVersion" : "4.0.1",
  "mapping" : [
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
    },
    {
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    },
    {
      "identity" : "loinc",
      "uri" : "http://loinc.org",
      "name" : "LOINC code for the element"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Patient",
  "baseDefinition" : "https://twcore.mohw.gov.tw/ig/twcore/StructureDefinition/Patient-twcore",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Patient",
        "path" : "Patient"
      },
      {
        "id" : "Patient.name",
        "path" : "Patient.name",
        "short" : "病患姓名，至少需要一組名與姓",
        "definition" : "病患姓名，包含名與姓，可有名子多個(以串列表示)",
        "min" : 1,
        "mustSupport" : true
      }
    ]
  }
}

```
