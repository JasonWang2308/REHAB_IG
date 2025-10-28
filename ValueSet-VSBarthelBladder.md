# 小便控制-選項 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **小便控制-選項**

## ValueSet: 小便控制-選項 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/ValueSet/VSBarthelBladder | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:VSBarthelBladder |

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
  "id" : "VSBarthelBladder",
  "url" : "http://example.org/ValueSet/VSBarthelBladder",
  "version" : "0.1.0",
  "name" : "VSBarthelBladder",
  "title" : "小便控制-選項",
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
            "display" : "能自己控制不會有失禁，或能自行使用並清潔尿套、尿袋。"
          },
          {
            "code" : "LA31626-7",
            "display" : "偶爾會失禁(每週不超過一次)或尿急(無法等待放好便盆或及時趕到廁 所)或需要他人協助處理尿套。"
          },
          {
            "code" : "LA31628-3",
            "display" : "失禁，無法自己控制且需他人處理。"
          }
        ]
      }
    ]
  }
}

```
