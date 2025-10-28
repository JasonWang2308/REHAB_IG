# 移位-選項 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **移位-選項**

## ValueSet: 移位-選項 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/ValueSet/VSBarthelTransfer | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:VSBarthelTransfer |

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
  "id" : "VSBarthelTransfer",
  "url" : "http://example.org/ValueSet/VSBarthelTransfer",
  "version" : "0.1.0",
  "name" : "VSBarthelTransfer",
  "title" : "移位-選項",
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
            "code" : "LA12302-8",
            "display" : "整個過程可獨立完成。"
          },
          {
            "code" : "LA31635-8",
            "display" : "移動身體時需要稍微協助、給予提醒、安全監督。"
          },
          {
            "code" : "LA31634-1",
            "display" : "可以自行坐起，但從床上坐起時或移動身體時需要他人協助。"
          },
          {
            "code" : "LA31633-3",
            "display" : "不會自己移動。"
          }
        ]
      }
    ]
  }
}

```
