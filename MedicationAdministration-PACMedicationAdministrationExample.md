# PAC用藥資料範例 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PAC用藥資料範例**

## Example MedicationAdministration: PAC用藥資料範例

Profile: [Medication Administration](StructureDefinition-MyMedicationAdministration.md)

**status**: Completed

**medication**: 阿莫西林 500mg

**subject**: [Patient/example](Patient/example)

**effective**: 2025-10-16 10:00:00+0800



## Resource Content

```json
{
  "resourceType" : "MedicationAdministration",
  "id" : "PACMedicationAdministrationExample",
  "meta" : {
    "profile" : [
      "http://example.org/StructureDefinition/MyMedicationAdministration"
    ]
  },
  "status" : "completed",
  "medicationCodeableConcept" : {
    "text" : "阿莫西林 500mg"
  },
  "subject" : {
    "reference" : "Patient/example"
  },
  "effectiveDateTime" : "2025-10-16T10:00:00+08:00"
}

```
