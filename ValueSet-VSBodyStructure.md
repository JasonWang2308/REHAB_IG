# 身體部位與結構對應之Snomed CT 代碼 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **身體部位與結構對應之Snomed CT 代碼**

## ValueSet: 身體部位與結構對應之Snomed CT 代碼 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/ValueSet/VSBodyStructure | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:VSBodyStructure |

 
收錄復健可能會使用到的身體部位代碼 

 **References** 

This value set is not used here; it may be used elsewhere (e.g. specifications and/or implementations that use this content)

### Logical Definition (CLD)

 

### Expansion

Expansion from tx.fhir.org based on SNOMED CT International edition 01-2月 2025

This value set contains 6 concepts

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
  "id" : "VSBodyStructure",
  "url" : "http://example.org/ValueSet/VSBodyStructure",
  "version" : "0.1.0",
  "name" : "VSBodyStructure",
  "title" : "身體部位與結構對應之Snomed CT 代碼",
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
  "description" : "收錄復健可能會使用到的身體部位代碼",
  "compose" : {
    "include" : [
      {
        "system" : "http://snomed.info/sct",
        "concept" : [
          {
            "code" : "91775009",
            "display" : "左側肩"
          },
          {
            "code" : "5951000",
            "display" : "左側手腕"
          },
          {
            "code" : "85151006",
            "display" : "左手"
          },
          {
            "code" : "91774008",
            "display" : "右側肩"
          },
          {
            "code" : "9736006",
            "display" : "右側手腕"
          },
          {
            "code" : "78791008",
            "display" : "右手"
          }
        ]
      }
    ]
  }
}

```
