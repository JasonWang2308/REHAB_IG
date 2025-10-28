# 健康照護服務提供者角色資料範例 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **健康照護服務提供者角色資料範例**

## Example PractitionerRole: 健康照護服務提供者角色資料範例

Profile: [PractitionerRole](StructureDefinition-PractitionerRole.md)

**active**: true

**practitioner**: [Practitioner 小姐 李 (official)](Practitioner-ot-therapist-001.md)

**organization**: [Organization 台灣健康醫院](Organization-OrganizationExample.md)

**code**: Doctor

**specialty**: General medicine



## Resource Content

```json
{
  "resourceType" : "PractitionerRole",
  "id" : "PractitionerRoleExample",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/PractitionerRole"]
  },
  "active" : true,
  "practitioner" : {
    "reference" : "Practitioner/ot-therapist-001"
  },
  "organization" : {
    "reference" : "Organization/OrganizationExample"
  },
  "code" : [
    {
      "coding" : [
        {
          "system" : "http://terminology.hl7.org/CodeSystem/v2-0286",
          "code" : "DO",
          "display" : "Doctor"
        }
      ]
    }
  ],
  "specialty" : [
    {
      "coding" : [
        {
          "system" : "http://snomed.info/sct",
          "code" : "394802001",
          "display" : "General medicine"
        }
      ]
    }
  ]
}

```
