# 健康狀態篩檢與評估範例 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **健康狀態篩檢與評估範例**

## Example Observation: 健康狀態篩檢與評估範例

Profile: [Observation Screening Assessment](StructureDefinition-ObservationScreeningAssessment.md)

**status**: Final

**category**: Survey

**code**: Health Status Screening

**subject**: [Patient/example](Patient/example)



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "ObservationScreeningAssessmentExample",
  "meta" : {
    "profile" : [
      "http://example.org/StructureDefinition/ObservationScreeningAssessment"
    ]
  },
  "status" : "final",
  "category" : [
    {
      "coding" : [
        {
          "system" : "http://terminology.hl7.org/CodeSystem/observation-category",
          "code" : "survey"
        }
      ]
    }
  ],
  "code" : {
    "coding" : [
      {
        "system" : "http://loinc.org",
        "display" : "Health Status Screening"
      }
    ]
  },
  "subject" : {
    "reference" : "Patient/example"
  }
}

```
