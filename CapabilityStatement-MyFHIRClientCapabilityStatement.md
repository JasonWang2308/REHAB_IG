# My FHIR Client Capability Statement - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **My FHIR Client Capability Statement**

## CapabilityStatement: My FHIR Client Capability Statement 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/CapabilityStatement/MyFHIRClient | *Version*:0.1.0 |
| Active as of 2025-10-25 | *Computable Name*:MyFHIRClientCapabilityStatement |

 
此 CapabilityStatement 定義了用戶端（Client）應支援的 FHIR RESTful API 功能。用戶端建議應該（SHOULD）使用伺服端能力聲明中的查詢參數，支援讀取和查詢一個或多個 FHIR Profile。 

 [Raw OpenAPI-Swagger Definition file](MyFHIRClientCapabilityStatement.openapi.json) | [Download](MyFHIRClientCapabilityStatement.openapi.json) 

## My FHIR Client Capability Statement

* Implementation Guide Version: 0.1.0 
* FHIR Version: 4.0.1 
* Supported Formats: `json`, `xml`
* Supported Patch Formats: `application/json-patch+json`
* Published on: 2025-10-25 
* Published by: Example Publisher 

> **Note to Implementers: FHIR Capabilities**Any FHIR capability may be 'allowed' by the system unless explicitly marked as 'SHALL NOT'. A few items are marked as MAY in the Implementation Guide to highlight their potential relevance to the use case.

## FHIR RESTful Capabilities

### Mode: client

用戶端建議應該（SHOULD）使用伺服端能力聲明中的查詢參數，支援讀取和查詢一個或多個 Profile。系統互動能力：可能可以（MAY）支援交易（transaction）、批次（batch）與查詢系統（search-system）。

### Capabilities by Resource/Profile

#### Summary

The summary table lists the resources that are part of this configuration, and for each resource it lists:

* The relevant profiles (if any)
* The interactions supported by each resource (**R**ead, **S**earch, **U**pdate, and **C**reate, are always shown, while **VR**ead, **P**atch, **D**elete, **H**istory on **I**nstance, or **H**istory on **T**ype are only present if at least one of the resources has support for them.
* The required, recommended, and some optional search parameters (if any).
* The linked resources enabled for `_include`
* The other resources enabled for `_revinclude`
* The operations on the resource (if any)

| | | | | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| [Bundle](#Bundle1-1) | [http://hl7.org/fhir/StructureDefinition/Bundle](http://hl7.org/fhir/R4/bundle.html) | Y | Y |  |  | _id, identifier |  |  |  |
| [CarePlan](#CarePlan1-2) | [http://hl7.org/fhir/StructureDefinition/CarePlan](http://hl7.org/fhir/R4/careplan.html) | Y | Y |  |  | patient, category, date, status |  |  |  |
| [Condition](#Condition1-3) | [http://hl7.org/fhir/StructureDefinition/Condition](http://hl7.org/fhir/R4/condition.html) | Y | Y |  |  | _id, clinical-status, code, subject, onset-date, abatement-date, severity |  |  |  |
| [Encounter](#Encounter1-4) | [http://hl7.org/fhir/StructureDefinition/Encounter](http://hl7.org/fhir/R4/encounter.html) | Y | Y |  |  | _id, class, date, identifier, location, subject, status |  |  |  |
| [Goal](#Goal1-5) | [http://hl7.org/fhir/StructureDefinition/Goal](http://hl7.org/fhir/R4/goal.html) | Y | Y |  |  | patient, lifecycle-status, target-date, description |  |  |  |
| [MedicationAdministration](#MedicationAdministration1-6) | [http://hl7.org/fhir/StructureDefinition/MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html) | Y | Y |  |  | code, identifier, medication, patient, status, context, device, effective-time, performer, reason-given, reason-not-given, request, subject |  |  |  |
| [Observation](#Observation1-7) | [http://hl7.org/fhir/StructureDefinition/Observation](http://hl7.org/fhir/R4/observation.html) | Y | Y |  |  | _id, category, code, date, performer, status, subject, patient, _lastUpdated |  |  |  |
| [Organization](#Organization1-8) | [http://hl7.org/fhir/StructureDefinition/Organization](http://hl7.org/fhir/R4/organization.html) | Y | Y |  |  | _id, identifier, name, type |  |  |  |
| [Patient](#Patient1-9) | [http://hl7.org/fhir/StructureDefinition/Patient](http://hl7.org/fhir/R4/patient.html) | Y | Y |  |  | _id, birthdate, gender, identifier, name |  |  | `$everything` |
| [Practitioner](#Practitioner1-10) | [http://hl7.org/fhir/StructureDefinition/Practitioner](http://hl7.org/fhir/R4/practitioner.html) | Y | Y |  |  | _id, identifier, name |  |  |  |
| [PractitionerRole](#PractitionerRole1-11) | [http://hl7.org/fhir/StructureDefinition/PractitionerRole](http://hl7.org/fhir/R4/practitionerrole.html) | Y | Y |  |  | _id, identifier, specialty |  |  |  |
| [Procedure](#Procedure1-12) | [http://hl7.org/fhir/StructureDefinition/Procedure](http://hl7.org/fhir/R4/procedure.html) | Y | Y |  |  | _id, code, status, subject, date |  |  |  |
| [Questionnaire](#Questionnaire1-13) | [http://hl7.org/fhir/StructureDefinition/Questionnaire](http://hl7.org/fhir/R4/questionnaire.html) | Y | Y |  |  | identifier, title |  |  |  |
| [QuestionnaireResponse](#QuestionnaireResponse1-14) | [http://hl7.org/fhir/StructureDefinition/QuestionnaireResponse](http://hl7.org/fhir/R4/questionnaireresponse.html) | Y | Y | Y | Y | _id, patient, status, authored, questionnaire, subject |  |  | `$extract` |

-------

#### Resource Conformance: SHOULD Bundle

Base System Profile

[Bundle](http://hl7.org/fhir/R4/bundle.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD CarePlan

Base System Profile

[CarePlan](http://hl7.org/fhir/R4/careplan.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD Condition

Base System Profile

[Condition](http://hl7.org/fhir/R4/condition.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD Encounter

Base System Profile

[Encounter](http://hl7.org/fhir/R4/encounter.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD Goal

Base System Profile

[Goal](http://hl7.org/fhir/R4/goal.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD MedicationAdministration

Base System Profile

[MedicationAdministration](http://hl7.org/fhir/R4/medicationadministration.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD Observation

Base System Profile

[Observation](http://hl7.org/fhir/R4/observation.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD Organization

Base System Profile

[Organization](http://hl7.org/fhir/R4/organization.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD Patient

Base System Profile

[Patient](http://hl7.org/fhir/R4/patient.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

Extended Operations


#### Resource Conformance: SHOULD Practitioner

Base System Profile

[Practitioner](http://hl7.org/fhir/R4/practitioner.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD PractitionerRole

Base System Profile

[PractitionerRole](http://hl7.org/fhir/R4/practitionerrole.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD Procedure

Base System Profile

[Procedure](http://hl7.org/fhir/R4/procedure.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD Questionnaire

Base System Profile

[Questionnaire](http://hl7.org/fhir/R4/questionnaire.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`.

Search Parameters


 

#### Resource Conformance: SHOULD QuestionnaireResponse

Base System Profile

[QuestionnaireResponse](http://hl7.org/fhir/R4/questionnaireresponse.html)

Profile Conformance

**SHOULD**

Reference Policy

Interaction summary

* **SHOULD** support `read`, `search-type`, `create`, `update`.

Search Parameters


 

Extended Operations




## Resource Content

```json
{
  "resourceType" : "CapabilityStatement",
  "id" : "MyFHIRClientCapabilityStatement",
  "url" : "http://example.org/fhir/CapabilityStatement/MyFHIRClient",
  "version" : "0.1.0",
  "name" : "MyFHIRClientCapabilityStatement",
  "title" : "My FHIR Client Capability Statement",
  "status" : "active",
  "experimental" : false,
  "date" : "2025-10-25",
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
  "description" : "此 CapabilityStatement 定義了用戶端（Client）應支援的 FHIR RESTful API 功能。用戶端建議應該（SHOULD）使用伺服端能力聲明中的查詢參數，支援讀取和查詢一個或多個 FHIR Profile。",
  "kind" : "requirements",
  "fhirVersion" : "4.0.1",
  "format" : ["json", "xml"],
  "patchFormat" : ["application/json-patch+json"],
  "rest" : [
    {
      "mode" : "client",
      "documentation" : "用戶端建議應該（SHOULD）使用伺服端能力聲明中的查詢參數，支援讀取和查詢一個或多個 Profile。系統互動能力：可能可以（MAY）支援交易（transaction）、批次（batch）與查詢系統（search-system）。",
      "resource" : [
        {
          "type" : "Bundle",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Bundle",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/Bundle-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "identifier",
              "definition" : "http://example.org/fhir/SearchParameter/Bundle-identifier",
              "type" : "token"
            }
          ]
        },
        {
          "type" : "CarePlan",
          "profile" : "http://hl7.org/fhir/StructureDefinition/CarePlan",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "patient",
              "definition" : "http://example.org/fhir/SearchParameter/CarePlan-patient",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "category",
              "definition" : "http://example.org/fhir/SearchParameter/CarePlan-category",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "date",
              "definition" : "http://example.org/fhir/SearchParameter/CarePlan-date",
              "type" : "date"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "status",
              "definition" : "http://example.org/fhir/SearchParameter/CarePlan-status",
              "type" : "token"
            }
          ]
        },
        {
          "type" : "Condition",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Condition",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/Condition-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "clinical-status",
              "definition" : "http://example.org/fhir/SearchParameter/Condition-clinical-status",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "code",
              "definition" : "http://example.org/fhir/SearchParameter/Condition-code",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "subject",
              "definition" : "http://example.org/fhir/SearchParameter/Condition-subject",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "onset-date",
              "definition" : "http://example.org/fhir/SearchParameter/Condition-onset-date",
              "type" : "date"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "abatement-date",
              "definition" : "http://example.org/fhir/SearchParameter/Condition-abatement-date",
              "type" : "date"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "severity",
              "definition" : "http://example.org/fhir/SearchParameter/Condition-severity",
              "type" : "token"
            }
          ]
        },
        {
          "type" : "Encounter",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Encounter",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/Encounter-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "class",
              "definition" : "http://example.org/fhir/SearchParameter/Encounter-class",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "date",
              "definition" : "http://example.org/fhir/SearchParameter/Encounter-date",
              "type" : "date"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "identifier",
              "definition" : "http://example.org/fhir/SearchParameter/Encounter-identifier",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "location",
              "definition" : "http://example.org/fhir/SearchParameter/Encounter-location",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "subject",
              "definition" : "http://example.org/fhir/SearchParameter/Encounter-subject",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "status",
              "definition" : "http://example.org/fhir/SearchParameter/Encounter-status",
              "type" : "token"
            }
          ]
        },
        {
          "type" : "Goal",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Goal",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "patient",
              "definition" : "http://example.org/fhir/SearchParameter/Goal-patient",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "lifecycle-status",
              "definition" : "http://example.org/fhir/SearchParameter/Goal-lifecycle-status",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "target-date",
              "definition" : "http://example.org/fhir/SearchParameter/Goal-target-date",
              "type" : "date"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "description",
              "definition" : "http://example.org/fhir/SearchParameter/Goal-description",
              "type" : "token"
            }
          ]
        },
        {
          "type" : "MedicationAdministration",
          "profile" : "http://hl7.org/fhir/StructureDefinition/MedicationAdministration",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "code",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-code",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "identifier",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-identifier",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "medication",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-medication",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "patient",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-patient",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "status",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-status",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "context",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-context",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "device",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-device",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "effective-time",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-effective-time",
              "type" : "date"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "performer",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-performer",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "reason-given",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-reason-given",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "reason-not-given",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-reason-not-given",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "request",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-request",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "subject",
              "definition" : "http://example.org/fhir/SearchParameter/MedicationAdministration-subject",
              "type" : "reference"
            }
          ]
        },
        {
          "type" : "Observation",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Observation",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/Observation-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "category",
              "definition" : "http://example.org/fhir/SearchParameter/Observation-category",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "code",
              "definition" : "http://example.org/fhir/SearchParameter/Observation-code",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "date",
              "definition" : "http://example.org/fhir/SearchParameter/Observation-date",
              "type" : "date"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "performer",
              "definition" : "http://example.org/fhir/SearchParameter/Observation-performer",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "status",
              "definition" : "http://example.org/fhir/SearchParameter/Observation-status",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "subject",
              "definition" : "http://example.org/fhir/SearchParameter/Observation-subject",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "patient",
              "definition" : "http://example.org/fhir/SearchParameter/Observation-patient",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_lastUpdated",
              "definition" : "http://example.org/fhir/SearchParameter/Observation-_lastUpdated",
              "type" : "date"
            }
          ]
        },
        {
          "type" : "Organization",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Organization",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/Organization-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "identifier",
              "definition" : "http://example.org/fhir/SearchParameter/Organization-identifier",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "name",
              "definition" : "http://example.org/fhir/SearchParameter/Organization-name",
              "type" : "string"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "type",
              "definition" : "http://example.org/fhir/SearchParameter/Organization-type",
              "type" : "token"
            }
          ]
        },
        {
          "type" : "Patient",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Patient",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/Patient-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "birthdate",
              "definition" : "http://example.org/fhir/SearchParameter/Patient-birthdate",
              "type" : "date"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "gender",
              "definition" : "http://example.org/fhir/SearchParameter/Patient-gender",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "identifier",
              "definition" : "http://example.org/fhir/SearchParameter/Patient-identifier",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "name",
              "definition" : "http://example.org/fhir/SearchParameter/Patient-name",
              "type" : "string"
            }
          ],
          "operation" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "everything",
              "definition" : "http://hl7.org/fhir/OperationDefinition/Patient-everything"
            }
          ]
        },
        {
          "type" : "Practitioner",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Practitioner",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/Practitioner-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "identifier",
              "definition" : "http://example.org/fhir/SearchParameter/Practitioner-identifier",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "name",
              "definition" : "http://example.org/fhir/SearchParameter/Practitioner-name",
              "type" : "string"
            }
          ]
        },
        {
          "type" : "PractitionerRole",
          "profile" : "http://hl7.org/fhir/StructureDefinition/PractitionerRole",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/PractitionerRole-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "identifier",
              "definition" : "http://example.org/fhir/SearchParameter/PractitionerRole-identifier",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "specialty",
              "definition" : "http://example.org/fhir/SearchParameter/PractitionerRole-specialty",
              "type" : "token"
            }
          ]
        },
        {
          "type" : "Procedure",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Procedure",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/Procedure-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "code",
              "definition" : "http://example.org/fhir/SearchParameter/Procedure-code",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "status",
              "definition" : "http://example.org/fhir/SearchParameter/Procedure-status",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "subject",
              "definition" : "http://example.org/fhir/SearchParameter/Procedure-subject",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "date",
              "definition" : "http://example.org/fhir/SearchParameter/Procedure-date",
              "type" : "date"
            }
          ]
        },
        {
          "type" : "Questionnaire",
          "profile" : "http://hl7.org/fhir/StructureDefinition/Questionnaire",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "identifier",
              "definition" : "http://example.org/fhir/SearchParameter/Questionnaire-identifier",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "title",
              "definition" : "http://example.org/fhir/SearchParameter/Questionnaire-title",
              "type" : "string"
            }
          ]
        },
        {
          "type" : "QuestionnaireResponse",
          "profile" : "http://hl7.org/fhir/StructureDefinition/QuestionnaireResponse",
          "_profile" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                "valueCode" : "SHOULD"
              }
            ]
          },
          "interaction" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "read"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "search-type"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "create"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "code" : "update"
            }
          ],
          "searchParam" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "_id",
              "definition" : "http://example.org/fhir/SearchParameter/QuestionnaireResponse-_id",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "patient",
              "definition" : "http://example.org/fhir/SearchParameter/QuestionnaireResponse-patient",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "status",
              "definition" : "http://example.org/fhir/SearchParameter/QuestionnaireResponse-status",
              "type" : "token"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "authored",
              "definition" : "http://example.org/fhir/SearchParameter/QuestionnaireResponse-authored",
              "type" : "date"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "questionnaire",
              "definition" : "http://example.org/fhir/SearchParameter/QuestionnaireResponse-questionnaire",
              "type" : "reference"
            },
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "subject",
              "definition" : "http://example.org/fhir/SearchParameter/QuestionnaireResponse-subject",
              "type" : "reference"
            }
          ],
          "operation" : [
            {
              "extension" : [
                {
                  "url" : "http://hl7.org/fhir/StructureDefinition/capabilitystatement-expectation",
                  "valueCode" : "SHOULD"
                }
              ],
              "name" : "extract",
              "definition" : "http://hl7.org/fhir/uv/sdc/OperationDefinition/QuestionnaireResponse-extract",
              "documentation" : "用戶端應支援 $extract 操作以：\n• 將已完成的問卷回應轉換為結構化 FHIR 資源\n• 支援 Observation 提取（計分、測量）\n• 支援資源 Bundle 提取（複雜資料模型）\n• 自動計算衍生欄位（如得分）\n\n調用例：\nPOST /QuestionnaireResponse/qr123/$extract\n返回值：\n{\n  \"resourceType\": \"Bundle\",\n  \"type\": \"transaction\",\n  \"entry\": [\n    {\n      \"resource\": {\n        \"resourceType\": \"Observation\",\n        \"code\": { \"coding\": [{ \"code\": \"depression-score\" }] },\n        \"value\": { \"integer\": 15 }\n      }\n    }\n  ]\n}\n\n這是 SDC 工作流的關鍵步驟"
            }
          ]
        }
      ]
    }
  ]
}

```
