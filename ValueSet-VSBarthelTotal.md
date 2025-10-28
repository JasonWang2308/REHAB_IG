# Barthel Index 總值集 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Barthel Index 總值集**

## ValueSet: Barthel Index 總值集 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/ValueSet/VSBarthelTotal | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:VSBarthelTotal |

 
整合 Barthel Index 各題之所有選項值集 

 **References** 

This value set is not used here; it may be used elsewhere (e.g. specifications and/or implementations that use this content)

### Logical Definition (CLD)

This value set includes codes based on the following rules:

* Import all the codes that are contained in the intersection of [進食-選項](ValueSet-VSBarthelFeeding.md)
* Import all the codes that are contained in the intersection of [個人衛生-選項](ValueSet-VSBarthelGrooming.md)
* Import all the codes that are contained in the intersection of [上廁所-選項](ValueSet-VSBarthelToiletUse.md)
* Import all the codes that are contained in the intersection of [洗澡-選項](ValueSet-VSBarthelBathing.md)
* Import all the codes that are contained in the intersection of [穿脫衣服-選項](ValueSet-VSBarthelDressing.md)
* Import all the codes that are contained in the intersection of [大便控制-選項](ValueSet-VSBarthelBowels.md)
* Import all the codes that are contained in the intersection of [小便控制-選項](ValueSet-VSBarthelBladder.md)
* Import all the codes that are contained in the intersection of [平地行走-選項](ValueSet-VSBarthelMobility.md)
* Import all the codes that are contained in the intersection of [上下樓梯-選項](ValueSet-VSBarthelStairs.md)
* Import all the codes that are contained in the intersection of [移位-選項](ValueSet-VSBarthelTransfer.md)

 

### Expansion

Expansion from tx.fhir.org based on:

* Loinc v2.81
* [valueset 洗澡-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelBathing.md)
* [valueset 小便控制-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelBladder.md)
* [valueset 大便控制-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelBowels.md)
* [valueset 穿脫衣服-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelDressing.md)
* [valueset 進食-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelFeeding.md)
* [valueset 個人衛生-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelGrooming.md)
* [valueset 平地行走-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelMobility.md)
* [valueset 上下樓梯-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelStairs.md)
* [valueset 上廁所-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelToiletUse.md)
* [valueset 移位-選項 v0.1.0 (ValueSet)](ValueSet-VSBarthelTransfer.md)

This value set contains 23 concepts

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
  "id" : "VSBarthelTotal",
  "url" : "http://example.org/ValueSet/VSBarthelTotal",
  "version" : "0.1.0",
  "name" : "VSBarthelTotal",
  "title" : "Barthel Index 總值集",
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
  "description" : "整合 Barthel Index 各題之所有選項值集",
  "compose" : {
    "include" : [
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelFeeding"]
      },
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelGrooming"]
      },
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelToiletUse"]
      },
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelBathing"]
      },
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelDressing"]
      },
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelBowels"]
      },
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelBladder"]
      },
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelMobility"]
      },
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelStairs"]
      },
      {
        "valueSet" : ["http://example.org/ValueSet/VSBarthelTransfer"]
      }
    ]
  }
}

```
