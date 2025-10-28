# ARAT評估會期 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ARAT評估會期**

## Example Encounter: ARAT評估會期

Profile: [Encounter](StructureDefinition-Encounter.md)

**status**: Finished

**class**: [ActCode AMB](http://terminology.hl7.org/6.5.0/CodeSystem-v3-ActCode.html#v3-ActCode-AMB): 門診

**type**: 職能治療評估

**subject**: [先生 張 (official) Male, DoB: 1965-03-15 ( http://example.org/mrn#12345)](Patient-stroke-patient-001.md)

### Participants

| | |
| :--- | :--- |
| - | **Individual** |
| * | [Practitioner 小姐 李 (official)](Practitioner-ot-therapist-001.md) |

**period**: 2025-10-11 14:00:00+0800 --> 2025-10-11 15:00:00+0800

**reasonCode**: 中風後復健



## Resource Content

```json
{
  "resourceType" : "Encounter",
  "id" : "arat-assessment-encounter-001",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/Encounter"]
  },
  "status" : "finished",
  "class" : {
    "system" : "http://terminology.hl7.org/CodeSystem/v3-ActCode",
    "code" : "AMB",
    "display" : "門診"
  },
  "type" : [
    {
      "coding" : [
        {
          "system" : "http://snomed.info/sct",
          "code" : "410155007",
          "display" : "職能治療評估"
        }
      ]
    }
  ],
  "subject" : {
    "reference" : "Patient/stroke-patient-001"
  },
  "participant" : [
    {
      "individual" : {
        "reference" : "Practitioner/ot-therapist-001"
      }
    }
  ],
  "period" : {
    "start" : "2025-10-11T14:00:00+08:00",
    "end" : "2025-10-11T15:00:00+08:00"
  },
  "reasonCode" : [
    {
      "coding" : [
        {
          "system" : "http://snomed.info/sct",
          "code" : "230690007",
          "display" : "中風後復健"
        }
      ]
    }
  ]
}

```
