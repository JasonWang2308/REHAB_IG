# 項目測試時間 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **項目測試時間**

## Extension: 項目測試時間 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/test-time-extension | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:TestTimeExtension |

記錄單一測試項目的完成時間

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [ARAT上肢功能評估問卷回覆](StructureDefinition-ARATQuestionnaireResponse.md) and [WMFT上肢功能評估問卷回覆](StructureDefinition-WMFTQuestionnaireResponse.md)
* Examples for this Extension: [Bundle/arat-bundle-001](Bundle-arat-bundle-001.md), [QuestionnaireResponse/WMFTQuestionnaireResponseExample](QuestionnaireResponse-WMFTQuestionnaireResponseExample.md) and [QuestionnaireResponse/arat-response-example-001](QuestionnaireResponse-arat-response-example-001.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/test-time-extension)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-test-time-extension.csv), [Excel](StructureDefinition-test-time-extension.xlsx), [Schematron](StructureDefinition-test-time-extension.sch) 

#### Constraints



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "test-time-extension",
  "url" : "http://example.org/StructureDefinition/test-time-extension",
  "version" : "0.1.0",
  "name" : "TestTimeExtension",
  "title" : "項目測試時間",
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
  "description" : "記錄單一測試項目的完成時間",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    }
  ],
  "kind" : "complex-type",
  "abstract" : false,
  "context" : [
    {
      "type" : "element",
      "expression" : "QuestionnaireResponse.item"
    }
  ],
  "type" : "Extension",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Extension",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Extension",
        "path" : "Extension",
        "short" : "項目測試時間",
        "definition" : "記錄單一測試項目的完成時間"
      },
      {
        "id" : "Extension.extension",
        "path" : "Extension.extension",
        "max" : "0"
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://example.org/StructureDefinition/test-time-extension"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "type" : [
          {
            "code" : "decimal"
          }
        ]
      }
    ]
  }
}

```
