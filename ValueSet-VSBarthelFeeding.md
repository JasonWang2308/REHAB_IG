# 進食-選項 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **進食-選項**

## ValueSet: 進食-選項 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/ValueSet/VSBarthelFeeding | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:VSBarthelFeeding |

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
  "id" : "VSBarthelFeeding",
  "url" : "http://example.org/ValueSet/VSBarthelFeeding",
  "version" : "0.1.0",
  "name" : "VSBarthelFeeding",
  "title" : "進食-選項",
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
            "display" : "自己在合理時間(約 10 秒鐘吃一口)可用筷子取食眼前的食物。若需進食輔具時，應會自行穿脫。"
          },
          {
            "code" : "LA31630-9",
            "display" : "需別人幫忙穿脫輔具或只會用湯匙進食。"
          },
          {
            "code" : "LA24937-7",
            "display" : "無法自行取食或耗費時間過長。"
          }
        ]
      }
    ]
  }
}

```
