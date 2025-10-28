# 機構資料範例 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **機構資料範例**

## Example Organization: 機構資料範例

Profile: [Organization](StructureDefinition-Organization.md)

**identifier**: `http://hospital.mohw.gov.tw/orgID`/12345678

**active**: true

**name**: 台灣健康醫院

**address**: 123 健康路 臺北市 中正區 100 



## Resource Content

```json
{
  "resourceType" : "Organization",
  "id" : "OrganizationExample",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/Organization"]
  },
  "identifier" : [
    {
      "system" : "http://hospital.mohw.gov.tw/orgID",
      "value" : "12345678"
    }
  ],
  "active" : true,
  "name" : "台灣健康醫院",
  "address" : [
    {
      "line" : ["123 健康路"],
      "city" : "臺北市",
      "state" : "中正區",
      "postalCode" : "100"
    }
  ]
}

```
