# 平地行走-選項 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **平地行走-選項**

## ValueSet: 平地行走-選項 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/ValueSet/VSBarthelMobility | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:VSBarthelMobility |

 **References** 

* Included into [VSBarthelTotal](ValueSet-VSBarthelTotal.md)
* [巴氏量表問卷回覆](StructureDefinition-BarthelQuestionnaireResponse.md)

### Logical Definition (CLD)

 

### Expansion

Expansion from tx.fhir.org based on Loinc v2.81

This value set contains 4 concepts

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
  "id" : "VSBarthelMobility",
  "url" : "http://example.org/ValueSet/VSBarthelMobility",
  "version" : "0.1.0",
  "name" : "VSBarthelMobility",
  "title" : "平地行走-選項",
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
            "code" : "LA31642-4",
            "display" : "使用或不使用輔具，皆可獨立行走 50 公尺以上。"
          },
          {
            "code" : "LA31641-6",
            "display" : "需他人稍微扶持或口頭指導才能行走 50 公尺以上。"
          },
          {
            "code" : "LA31640-8",
            "display" : "雖無法行走，但可以操作輪椅(包括轉彎、進門及接近桌子、床沿)並可 推行輪椅 50 公尺以上。"
          },
          {
            "code" : "LA31639-0",
            "display" : "完全無法自行行走，需別人幫忙推輪椅。"
          }
        ]
      }
    ]
  }
}

```
