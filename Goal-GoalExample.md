# 目標資料範例 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **目標資料範例**

## Example Goal: 目標資料範例

Profile: [Goal](StructureDefinition-Goal.md)

**lifecycleStatus**: Active

**category**: health-management

**description**: 控制血糖在目標範圍內

**subject**: [Patient/001](Patient/001)



## Resource Content

```json
{
  "resourceType" : "Goal",
  "id" : "GoalExample",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/Goal"]
  },
  "lifecycleStatus" : "active",
  "category" : [
    {
      "coding" : [
        {
          "system" : "http://terminology.hl7.org/CodeSystem/goal-category",
          "code" : "health-management"
        }
      ]
    }
  ],
  "description" : {
    "text" : "控制血糖在目標範圍內"
  },
  "subject" : {
    "reference" : "Patient/001"
  }
}

```
