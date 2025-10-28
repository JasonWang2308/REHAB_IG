# 復健治療師範例 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **復健治療師範例**

## Example Practitioner: 復健治療師範例

Profile: [Practitioner](StructureDefinition-Practitioner.md)

**identifier**: `http://hospital.mohw.gov.tw/docID`/A123456789

**active**: true

**name**: 小姐 李 (Official)

### Qualifications

| | | |
| :--- | :--- | :--- |
| - | **Code** | **Issuer** |
| * | 職能治療師 | 台灣職能治療師公會 |



## Resource Content

```json
{
  "resourceType" : "Practitioner",
  "id" : "ot-therapist-001",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/Practitioner"]
  },
  "identifier" : [
    {
      "system" : "http://hospital.mohw.gov.tw/docID",
      "value" : "A123456789"
    }
  ],
  "active" : true,
  "name" : [
    {
      "use" : "official",
      "family" : "李",
      "given" : ["小姐"]
    }
  ],
  "qualification" : [
    {
      "code" : {
        "coding" : [
          {
            "system" : "http://snomed.info/sct",
            "code" : "224609002",
            "display" : "職能治療師"
          }
        ]
      },
      "issuer" : {
        "display" : "台灣職能治療師公會"
      }
    }
  ]
}

```
