# 中風患者範例 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **中風患者範例**

## Example Patient: 中風患者範例

Profile: [Patient](StructureDefinition-Patient.md)

先生 張 (official) Male, DoB: 1965-03-15 ( http://example.org/mrn#12345)

-------

| | |
| :--- | :--- |
| Active: | true |
| Contact Detail | 台北市 台灣 |



## Resource Content

```json
{
  "resourceType" : "Patient",
  "id" : "stroke-patient-001",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/Patient"]
  },
  "identifier" : [
    {
      "system" : "http://example.org/mrn",
      "value" : "12345"
    }
  ],
  "active" : true,
  "name" : [
    {
      "use" : "official",
      "family" : "張",
      "given" : ["先生"]
    }
  ],
  "gender" : "male",
  "birthDate" : "1965-03-15",
  "address" : [
    {
      "city" : "台北市",
      "country" : "台灣"
    }
  ]
}

```
