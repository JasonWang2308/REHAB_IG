# 照護計畫資料範例 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **照護計畫資料範例**

## Example CarePlan: 照護計畫資料範例

Profile: [Care Plan](StructureDefinition-CarePlan.md)

**status**: Active

**intent**: Plan

**category**: Assessment and Plan of Treatment

**subject**: [Patient/001](Patient/001)



## Resource Content

```json
{
  "resourceType" : "CarePlan",
  "id" : "CarePlanExample",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/CarePlan"]
  },
  "status" : "active",
  "intent" : "plan",
  "category" : [
    {
      "coding" : [
        {
          "system" : "https://twcore.mohw.gov.tw/ig/twcore/CodeSystem/careplan-category-tw",
          "code" : "assess-plan"
        }
      ]
    }
  ],
  "subject" : {
    "reference" : "Patient/001"
  }
}

```
