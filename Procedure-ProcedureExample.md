# 介入資料範例 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **介入資料範例**

## Example Procedure: 介入資料範例

Profile: [PACProcedure](StructureDefinition-Procedure.md)

**status**: Completed

**code**: Appendectomy

**subject**: [Patient/001](Patient/001)

**performed**: 2025-10-09 10:00:00+0800



## Resource Content

```json
{
  "resourceType" : "Procedure",
  "id" : "ProcedureExample",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/Procedure"]
  },
  "status" : "completed",
  "code" : {
    "coding" : [
      {
        "system" : "http://snomed.info/sct",
        "code" : "80146002",
        "display" : "Appendectomy"
      }
    ]
  },
  "subject" : {
    "reference" : "Patient/001"
  },
  "performedDateTime" : "2025-10-09T10:00:00+08:00"
}

```
