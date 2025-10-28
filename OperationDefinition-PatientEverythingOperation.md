# Patient Everything Operation - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Patient Everything Operation**

## OperationDefinition: Patient Everything Operation 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/OperationDefinition/Patient-everything | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:PatientEverythingOperation |

 
取得該病人完整相關資源快照，回傳一個包含所有相關資源的Bundle 

URL: [base]/Patient/[id]/$everything

### Parameters

* **Use**: OUT
  * **Name**: return
  * **Scope**: 
  * **Cardinality**: 1..1
  * **Type**: [Bundle](http://hl7.org/fhir/R4/bundle.html)
  * **Binding**: 
  * **Documentation**: 包含所有相關資源的Bundle



## Resource Content

```json
{
  "resourceType" : "OperationDefinition",
  "id" : "PatientEverythingOperation",
  "url" : "http://example.org/fhir/OperationDefinition/Patient-everything",
  "version" : "0.1.0",
  "name" : "PatientEverythingOperation",
  "title" : "Patient Everything Operation",
  "status" : "active",
  "kind" : "operation",
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
  "description" : "取得該病人完整相關資源快照，回傳一個包含所有相關資源的Bundle",
  "code" : "everything",
  "resource" : ["Patient"],
  "system" : false,
  "type" : false,
  "instance" : true,
  "parameter" : [
    {
      "name" : "return",
      "use" : "out",
      "min" : 1,
      "max" : "1",
      "documentation" : "包含所有相關資源的Bundle",
      "type" : "Bundle"
    }
  ]
}

```
