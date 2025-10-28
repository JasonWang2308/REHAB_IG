# 評估問卷回覆 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **評估問卷回覆**

## Resource Profile: 評估問卷回覆 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/SPACQuestionnaireResponse | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:SPACQuestionnaireResponse |

 
問卷回覆的結構化定義，實際問回覆內容可參考Examples，可依據前者內容做為範本進行擴充 

**Usages:**

* Derived from this Profile: [ARAT上肢功能評估問卷回覆](StructureDefinition-ARATQuestionnaireResponse.md), [巴氏量表問卷回覆](StructureDefinition-BarthelQuestionnaireResponse.md), [FMAUE動作評估問卷回覆](StructureDefinition-FMAUEMotionQuestionnaireResponse.md), [FMAUE感覺評估問卷回覆](StructureDefinition-FMAUESensoryQuestionnaireResponse.md)...Show 5 more,[IADL評估問卷回覆](StructureDefinition-IADLQuestionnaireResponse.md),[MAS 量表問卷回覆](StructureDefinition-MASQuestionnaireResponse.md),[MMSE QuestionnaireResponse (scored)](StructureDefinition-MMSEQuestionnaireResponse.md),[MRCQuestionnaireResponse](StructureDefinition-MRCQuestionnaireResponse.md)and[WMFT上肢功能評估問卷回覆](StructureDefinition-WMFTQuestionnaireResponse.md)
* Examples for this Profile: [QuestionnaireResponse/FMAUEMotorQuestionnaireResponseExample](QuestionnaireResponse-FMAUEMotorQuestionnaireResponseExample.md), [QuestionnaireResponse/IDALQuestionnaireResponseInstance](QuestionnaireResponse-IDALQuestionnaireResponseInstance.md) and [QuestionnaireResponse/MRCQuestionnaireResponseExample](QuestionnaireResponse-MRCQuestionnaireResponseExample.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/SPACQuestionnaireResponse)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-SPACQuestionnaireResponse.csv), [Excel](StructureDefinition-SPACQuestionnaireResponse.xlsx), [Schematron](StructureDefinition-SPACQuestionnaireResponse.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "SPACQuestionnaireResponse",
  "url" : "http://example.org/StructureDefinition/SPACQuestionnaireResponse",
  "version" : "0.1.0",
  "name" : "SPACQuestionnaireResponse",
  "title" : "評估問卷回覆",
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
  "description" : "問卷回覆的結構化定義，實際問回覆內容可參考Examples，可依據前者內容做為範本進行擴充",
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
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "QuestionnaireResponse",
  "baseDefinition" : "http://hl7.org/fhir/uv/sdc/StructureDefinition/sdc-questionnaireresponse",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "QuestionnaireResponse",
        "path" : "QuestionnaireResponse"
      },
      {
        "id" : "QuestionnaireResponse.subject",
        "path" : "QuestionnaireResponse.subject",
        "min" : 1
      },
      {
        "id" : "QuestionnaireResponse.subject.reference",
        "path" : "QuestionnaireResponse.subject.reference",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.source",
        "path" : "QuestionnaireResponse.source",
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.source.reference",
        "path" : "QuestionnaireResponse.source.reference",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "QuestionnaireResponse.item",
        "path" : "QuestionnaireResponse.item",
        "min" : 1
      },
      {
        "id" : "QuestionnaireResponse.item.answer.extension:ordinalValue",
        "path" : "QuestionnaireResponse.item.answer.extension",
        "sliceName" : "ordinalValue",
        "mustSupport" : true
      }
    ]
  }
}

```
