# 大便控制-選項 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **大便控制-選項**

## ValueSet: 大便控制-選項 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/ValueSet/VSBarthelBowels | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:VSBarthelBowels |

 **References** 

* Included into [VSBarthelTotal](ValueSet-VSBarthelTotal.md)
* [巴氏量表問卷回覆](StructureDefinition-BarthelQuestionnaireResponse.md)

### Logical Definition (CLD)

 

### Expansion

Expansion from tx.fhir.org based on Loinc v2.81

This value set contains 3 concepts

-------

 Explanation of the columns that may appear on this page: 

| | |
| :--- | :--- |
| Level | A few code lists that FHIR defines are hierarchical - each code is assigned a level. In this scheme, some codes are under other codes, and imply that the code they are under also applies |
| System | The source of the definition of the code (when the value set draws in codes defined elsewhere) |
| Code | The code (used as the code in the resource instance) |
| Display | The display (used in the*display*element of a[Coding](http://hl7.org/fhir/R4/datatypes.html#Coding)). If there is no display, implementers should not simply display the code, but map the concept into their application |
| Definition | An explanation of the meaning of the concept |
| Comments | Additional notes about how to use the code |



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "VSBarthelBowels",
  "url" : "http://example.org/ValueSet/VSBarthelBowels",
  "version" : "0.1.0",
  "name" : "VSBarthelBowels",
  "title" : "大便控制-選項",
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
  "compose" : {
    "include" : [
      {
        "system" : "http://loinc.org",
        "concept" : [
          {
            "code" : "LA31625-9",
            "display" : "不會失禁，能自行灌腸或使用塞劑。"
          },
          {
            "code" : "LA31626-7",
            "display" : "偶爾會失禁(每週不超過一次)，需要他人協助使用灌腸或塞劑。"
          },
          {
            "code" : "LA31627-5",
            "display" : "失禁，無法自己控制且需他人處理。"
          }
        ]
      }
    ]
  }
}

```
