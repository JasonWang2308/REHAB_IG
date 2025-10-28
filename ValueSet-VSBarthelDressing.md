# 穿脫衣服-選項 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **穿脫衣服-選項**

## ValueSet: 穿脫衣服-選項 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/ValueSet/VSBarthelDressing | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:VSBarthelDressing |

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
  "id" : "VSBarthelDressing",
  "url" : "http://example.org/ValueSet/VSBarthelDressing",
  "version" : "0.1.0",
  "name" : "VSBarthelDressing",
  "title" : "穿脫衣服-選項",
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
            "code" : "LA31638-2",
            "display" : "能自己穿脫衣服、鞋子，自己扣釦子、上拉鍊或綁鞋帶。"
          },
          {
            "code" : "LA31637-4",
            "display" : "在別人協助下，可自己完成一半以上的動作。"
          },
          {
            "code" : "LA12304-4",
            "display" : "不會自己做。"
          }
        ]
      }
    ]
  }
}

```
