# MAS 分數 (0,1,1+,2,3,4) - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MAS 分數 (0,1,1+,2,3,4)**

## ValueSet: MAS 分數 (0,1,1+,2,3,4) 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/ValueSet/mas-score | *Version*:0.1.0 |
| Draft as of 2025-10-28 | *Computable Name*:VSMAScore |

 **References** 

* [MAS 量表問卷回覆](StructureDefinition-MASQuestionnaireResponse.md)
* [MAS評估量表](Questionnaire-MASQuestionnaireInstance.md)

### Logical Definition (CLD)

* Include all codes defined in `https://your-org.example/fhir/ig/rehab/CodeSystem/mas-score`version Not Stated (use latest from terminology server)

 

### Expansion

No Expansion for this valueset (Unknown Code System)

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
  "id" : "mas-score",
  "url" : "http://example.org/ValueSet/mas-score",
  "version" : "0.1.0",
  "name" : "VSMAScore",
  "title" : "MAS 分數 (0,1,1+,2,3,4)",
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
  "compose" : {
    "include" : [
      {
        "system" : "https://your-org.example/fhir/ig/rehab/CodeSystem/mas-score"
      }
    ]
  }
}

```
