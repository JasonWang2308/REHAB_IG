# Artifacts Summary - v0.1.0

* [**Table of Contents**](toc.md)
* **Artifacts Summary**

## Artifacts Summary

This page provides a list of the FHIR artifacts defined as part of this implementation guide.

### Behavior: Capability Statements 

The following artifacts define the specific capabilities that different types of systems are expected to have in order to comply with this implementation guide. Systems conforming to this implementation guide are expected to declare conformance to one or more of the following capability statements.

| | |
| :--- | :--- |
| [My FHIR Client Capability Statement](CapabilityStatement-MyFHIRClientCapabilityStatement.md) | 此 CapabilityStatement 定義了用戶端（Client）應支援的 FHIR RESTful API 功能。用戶端建議應該（SHOULD）使用伺服端能力聲明中的查詢參數，支援讀取和查詢一個或多個 FHIR Profile。 |
| [My FHIR Server Capability Statement](CapabilityStatement-MyFHIRServerCapabilityStatement.md) | 此 CapabilityStatement 定義了伺服端必須支援的 FHIR RESTful API 功能 |

### Behavior: Operation Definitions 

These are custom operations that can be supported by and/or invoked by systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [Patient Everything Operation](OperationDefinition-PatientEverythingOperation.md) | 取得該病人完整相關資源快照，回傳一個包含所有相關資源的Bundle |

### Behavior: Search Parameters 

These define the properties by which a RESTful server can be searched. They can also be used for sorting and including related resources.

| | |
| :--- | :--- |
| [BundleId](SearchParameter-BundleId.md) | 搜尋Bundle的_id參數 |
| [BundleIdentifier](SearchParameter-BundleIdentifier.md) | 搜尋Bundle的identifier參數 |
| [CarePlanCategory](SearchParameter-CarePlanCategory.md) | 搜尋CarePlan的category參數 |
| [CarePlanDate](SearchParameter-CarePlanDate.md) | 搜尋CarePlan的date參數 |
| [CarePlanPatient](SearchParameter-CarePlanPatient.md) | 搜尋CarePlan的patient參數 |
| [CarePlanStatus](SearchParameter-CarePlanStatus.md) | 搜尋CarePlan的status參數 |
| [ConditionAbatementdate](SearchParameter-ConditionAbatementdate.md) | 搜尋Condition的abatement-date參數 |
| [ConditionClinicalstatus](SearchParameter-ConditionClinicalstatus.md) | 搜尋Condition的clinical-status參數 |
| [ConditionCode](SearchParameter-ConditionCode.md) | 搜尋Condition的code參數 |
| [ConditionId](SearchParameter-ConditionId.md) | 搜尋Condition的_id參數 |
| [ConditionOnsetdate](SearchParameter-ConditionOnsetdate.md) | 搜尋Condition的onset-date參數 |
| [ConditionSeverity](SearchParameter-ConditionSeverity.md) | 搜尋Condition的severity參數 |
| [ConditionSubject](SearchParameter-ConditionSubject.md) | 搜尋Condition的subject參數 |
| [EncounterClass](SearchParameter-EncounterClass.md) | 搜尋Encounter的class參數 |
| [EncounterDate](SearchParameter-EncounterDate.md) | 搜尋Encounter的date參數 |
| [EncounterId](SearchParameter-EncounterId.md) | 搜尋Encounter的_id參數 |
| [EncounterIdentifier](SearchParameter-EncounterIdentifier.md) | 搜尋Encounter的identifier參數 |
| [EncounterLocation](SearchParameter-EncounterLocation.md) | 搜尋Encounter的location參數 |
| [EncounterStatus](SearchParameter-EncounterStatus.md) | 搜尋Encounter的status參數 |
| [EncounterSubject](SearchParameter-EncounterSubject.md) | 搜尋Encounter的subject參數 |
| [GoalDescription](SearchParameter-GoalDescription.md) | 搜尋Goal的description參數 |
| [GoalLifecyclestatus](SearchParameter-GoalLifecyclestatus.md) | 搜尋Goal的lifecycle-status參數 |
| [GoalPatient](SearchParameter-GoalPatient.md) | 搜尋Goal的patient參數 |
| [GoalTargetdate](SearchParameter-GoalTargetdate.md) | 搜尋Goal的target-date參數 |
| [MedicationAdministrationCode](SearchParameter-MedicationAdministrationCode.md) | Return administrations of this medication code |
| [MedicationAdministrationContext](SearchParameter-MedicationAdministrationContext.md) | Return administrations that share this encounter or episode of care |
| [MedicationAdministrationDevice](SearchParameter-MedicationAdministrationDevice.md) | Return administrations with this administration device identity |
| [MedicationAdministrationEffectivetime](SearchParameter-MedicationAdministrationEffectivetime.md) | Date administration happened (or did not happen) |
| [MedicationAdministrationIdentifier](SearchParameter-MedicationAdministrationIdentifier.md) | Return administrations with this external identifier |
| [MedicationAdministrationMedication](SearchParameter-MedicationAdministrationMedication.md) | Return administrations of this medication resource |
| [MedicationAdministrationPatient](SearchParameter-MedicationAdministrationPatient.md) | The identity of a patient to list administrations for |
| [MedicationAdministrationPerformer](SearchParameter-MedicationAdministrationPerformer.md) | The identity of the individual who administered the medication |
| [MedicationAdministrationReasongiven](SearchParameter-MedicationAdministrationReasongiven.md) | Reasons for administering the medication |
| [MedicationAdministrationReasonnotgiven](SearchParameter-MedicationAdministrationReasonnotgiven.md) | Reasons for not administering the medication |
| [MedicationAdministrationRequest](SearchParameter-MedicationAdministrationRequest.md) | The identity of a request to list administrations from |
| [MedicationAdministrationStatus](SearchParameter-MedicationAdministrationStatus.md) | MedicationAdministration event status (for example one of active/paused/completed/nullified) |
| [MedicationAdministrationSubject](SearchParameter-MedicationAdministrationSubject.md) | The identity of the individual or group to list administrations for |
| [ObservationCategory](SearchParameter-ObservationCategory.md) | 搜尋Observation的category參數 |
| [ObservationCode](SearchParameter-ObservationCode.md) | 搜尋Observation的code參數 |
| [ObservationDate](SearchParameter-ObservationDate.md) | 搜尋Observation的date參數 |
| [ObservationId](SearchParameter-ObservationId.md) | 搜尋Observation的_id參數 |
| [ObservationLastupdated](SearchParameter-ObservationLastupdated.md) | 搜尋Observation的_lastUpdated參數 |
| [ObservationPatient](SearchParameter-ObservationPatient.md) | 搜尋Observation的patient參數 |
| [ObservationPerformer](SearchParameter-ObservationPerformer.md) | 搜尋Observation的performer參數 |
| [ObservationStatus](SearchParameter-ObservationStatus.md) | 搜尋Observation的status參數 |
| [ObservationSubject](SearchParameter-ObservationSubject.md) | 搜尋Observation的subject參數 |
| [OrganizationId](SearchParameter-OrganizationId.md) | 搜尋Organization的_id參數 |
| [OrganizationIdentifier](SearchParameter-OrganizationIdentifier.md) | 搜尋Organization的identifier參數 |
| [OrganizationName](SearchParameter-OrganizationName.md) | 搜尋Organization的name參數 |
| [OrganizationType](SearchParameter-OrganizationType.md) | 搜尋Organization的type參數 |
| [PatientBirthdate](SearchParameter-PatientBirthdate.md) | 搜尋Patient的birthdate參數 |
| [PatientGender](SearchParameter-PatientGender.md) | 搜尋Patient的gender參數 |
| [PatientId](SearchParameter-PatientId.md) | 搜尋Patient的_id參數 |
| [PatientIdentifier](SearchParameter-PatientIdentifier.md) | 搜尋Patient的identifier參數 |
| [PatientName](SearchParameter-PatientName.md) | 搜尋Patient的name參數 |
| [PractitionerId](SearchParameter-PractitionerId.md) | 搜尋Practitioner的_id參數 |
| [PractitionerIdentifier](SearchParameter-PractitionerIdentifier.md) | 搜尋Practitioner的identifier參數 |
| [PractitionerName](SearchParameter-PractitionerName.md) | 搜尋Practitioner的name參數 |
| [PractitionerRoleId](SearchParameter-PractitionerRoleId.md) | 搜尋PractitionerRole的_id參數 |
| [PractitionerRoleIdentifier](SearchParameter-PractitionerRoleIdentifier.md) | 搜尋PractitionerRole的identifier參數 |
| [PractitionerRoleSpecialty](SearchParameter-PractitionerRoleSpecialty.md) | 搜尋PractitionerRole的specialty參數 |
| [ProcedureCode](SearchParameter-ProcedureCode.md) | 搜尋Procedure的code參數 |
| [ProcedureDate](SearchParameter-ProcedureDate.md) | 搜尋Procedure的date參數 |
| [ProcedureId](SearchParameter-ProcedureId.md) | 搜尋Procedure的_id參數 |
| [ProcedureStatus](SearchParameter-ProcedureStatus.md) | 搜尋Procedure的status參數 |
| [ProcedureSubject](SearchParameter-ProcedureSubject.md) | 搜尋Procedure的subject參數 |
| [QuestionnaireIdentifier](SearchParameter-QuestionnaireIdentifier.md) | 問卷識別碼 |
| [QuestionnaireLinkID](SearchParameter-QuestionnaireLinkID.md) | 問卷項目 |
| [QuestionnaireResponseAuthored](SearchParameter-QuestionnaireResponseAuthored.md) | 搜尋QuestionnaireResponse的authored參數 |
| [QuestionnaireResponseId](SearchParameter-QuestionnaireResponseId.md) | 搜尋QuestionnaireResponse的_id參數 |
| [QuestionnaireResponseLinkID](SearchParameter-QuestionnaireResponseLinkID.md) | 問卷標題 |
| [QuestionnaireResponsePatient](SearchParameter-QuestionnaireResponsePatient.md) | 搜尋QuestionnaireResponse的patient參數 |
| [QuestionnaireResponseQuestionnaire](SearchParameter-QuestionnaireResponseQuestionnaire.md) | 搜尋QuestionnaireResponse的questionnaire參數 |
| [QuestionnaireResponseStatus](SearchParameter-QuestionnaireResponseStatus.md) | 搜尋QuestionnaireResponse的status參數 |
| [QuestionnaireResponseSubject](SearchParameter-QuestionnaireResponseSubject.md) | 問卷回應主體 |
| [QuestionnaireTitle](SearchParameter-QuestionnaireTitle.md) | 問卷標題 |

### Structures: Questionnaires 

These define forms used by systems conforming to this implementation guide to capture or expose data to end users.

| | |
| :--- | :--- |
| [ARAT上肢功能評估問卷](Questionnaire-ARATQuestionnaireInstance.md) | ARAT上肢功能評估問卷的完整實例，根據Yozbatiran, Der-Yeghiaian, and Cramer(2008)建立，可提供實際使用 。亦可依據Profile: QuestionnaireProfile內容做為範本進行擴充 |
| [BBT評估量表](Questionnaire-BBTQuestionnaire.md) | 評估手部功能 |
| [Fugl-Meyer上肢動作評估問卷](Questionnaire-FMAUEMotorQuestionnaireInstance.md) | 衛福部Fugl-Meyer上肢動作評估問卷的完整實例，可提供實際使用。亦可依據Profile: QuestionnaireProfile內容做為範本進行擴充 |
| [Fugl-Meyer上肢感覺評估問卷](Questionnaire-FMAUESensoryQuestionnaireInstance.md) | 衛福部Fugl-Meyer上肢感覺評估問卷的完整實例，可提供實際使用。亦可依據Profile: QuestionnaireProfile內容做為範本進行擴充 |
| [IDAL評估問卷](Questionnaire-IDALQuestionnaireInstance.md) | IADL評估問卷 |
| [MAS評估量表](Questionnaire-MASQuestionnaireInstance.md) | 評估肌肉張力 |
| [MMSE評估量表](Questionnaire-MMSEQuestionnaireInstance.md) | 簡易心智狀況檢查表 (Mini-Mental State Examination, MMSE) |
| [MRC 評估量表](Questionnaire-MRCQuestionnaireInstance.md) | MRC肌力測試 (Medical Research Council Scale) |
| [WMFT上肢功能評估問卷](Questionnaire-WMFTQuestionnaireInstance.md) | WMFT上肢功能評估問卷的完整實例，根據Wolf et al., 1995; Whitall, Savin, Harris-Love, & Waller, 2006建立，可提供實際使用 。亦可依據Profile: QuestionnaireProfile內容做為範本進行擴充 |
| [巴氏量表](Questionnaire-BarthelQuestionnaireInstance.md) | 巴氏量表 (Barthel Index) |

### Structures: Resource Profiles 

These define constraints on FHIR resources for systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [ARAT上肢功能評估問卷回覆](StructureDefinition-ARATQuestionnaireResponse.md) | 針對ARAT上肢功能評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 |
| [BBTQR](StructureDefinition-bbt-questionnaire-response.md) | Box and Block Test (BBT) 評估量表問卷回覆 |
| [Bundle-評估資料回傳](StructureDefinition-ReponseBundle.md) | 此 Profile 定義了上肢功能評估資料須包含的資訊。 |
| [Care Plan](StructureDefinition-CarePlan.md) | 照護計畫 |
| [Encounter](StructureDefinition-Encounter.md) | 就醫事件的標準化定義。 |
| [FMAUE動作評估問卷回覆](StructureDefinition-FMAUEMotionQuestionnaireResponse.md) | 針對FMAUE上肢動作評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 |
| [FMAUE感覺評估問卷回覆](StructureDefinition-FMAUESensoryQuestionnaireResponse.md) | 針對FMAUE上肢感覺評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 |
| [Goal](StructureDefinition-Goal.md) | 目標的標準化定義。 |
| [IADL評估問卷回覆](StructureDefinition-IADLQuestionnaireResponse.md) | 針對IADL評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 |
| [MAS 量表問卷回覆](StructureDefinition-MASQuestionnaireResponse.md) | Modified Ashworth Scale (MAS) 評估量表問卷回覆 |
| [MMSE QuestionnaireResponse (scored)](StructureDefinition-MMSEQuestionnaireResponse.md) | MMSE 回覆：分數題逐題填答，總分需等於所有分數項目加總。 |
| [MRCQuestionnaireResponse](StructureDefinition-MRCQuestionnaireResponse.md) | MRC問卷回覆 |
| [Medication Administration](StructureDefinition-MyMedicationAdministration.md) | 用藥資料 |
| [Observation Screening Assessment](StructureDefinition-ObservationScreeningAssessment.md) | 健康狀態篩檢與評估 |
| [Organization](StructureDefinition-Organization.md) | 機構的標準化定義。 |
| [PACCarePlan](StructureDefinition-PACCarePlan.md) | PAC照護計畫的標準化定義的內容 |
| [PACCondition](StructureDefinition-PACCondition.md) | 進行患者上肢功能評估時的狀況資訊，應包含待評估身體部位或病徵。 |
| [PACProcedure](StructureDefinition-Procedure.md) | PAC介入的標準化定義。 |
| [Patient](StructureDefinition-Patient.md) | 病人的資料定義範例，包含姓名、識別碼等基本資訊 |
| [Practitioner](StructureDefinition-Practitioner.md) | 健康照護服務提供者的標準化定義。 |
| [PractitionerRole](StructureDefinition-PractitionerRole.md) | 健康照護服務提供者角色的標準化定義。 |
| [WMFT上肢功能評估問卷回覆](StructureDefinition-WMFTQuestionnaireResponse.md) | 針對WMFT上肢功能評估問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 |
| [巴氏量表問卷回覆](StructureDefinition-BarthelQuestionnaireResponse.md) | 針對巴氏量表問卷的QuestionnaireResponse Profile，強制回傳格式符合問卷結構 |
| [評估問卷](StructureDefinition-SPACQuestionnaire.md) | 評估問卷的結構化定義，實際問卷內容請參考Structure: Questionnaire，可依據前者內容做為範本進行擴充 |
| [評估問卷回覆](StructureDefinition-SPACQuestionnaireResponse.md) | 問卷回覆的結構化定義，實際問回覆內容可參考Examples，可依據前者內容做為範本進行擴充 |

### Structures: Extension Definitions 

These define constraints on FHIR data types for systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [項目測試時間](StructureDefinition-test-time-extension.md) | 記錄單一測試項目的完成時間 |

### Terminology: Value Sets 

These define sets of codes used by systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [Barthel Index 總值集](ValueSet-VSBarthelTotal.md) | 整合 Barthel Index 各題之所有選項值集 |
| [MAS 分數 (0,1,1+,2,3,4)](ValueSet-mas-score.md) |  |
| [上下樓梯-選項](ValueSet-VSBarthelStairs.md) |  |
| [上廁所-選項](ValueSet-VSBarthelToiletUse.md) |  |
| [個人衛生-選項](ValueSet-VSBarthelGrooming.md) |  |
| [大便控制-選項](ValueSet-VSBarthelBowels.md) |  |
| [小便控制-選項](ValueSet-VSBarthelBladder.md) |  |
| [平地行走-選項](ValueSet-VSBarthelMobility.md) |  |
| [洗澡-選項](ValueSet-VSBarthelBathing.md) |  |
| [移位-選項](ValueSet-VSBarthelTransfer.md) |  |
| [穿脫衣服-選項](ValueSet-VSBarthelDressing.md) |  |
| [評估側別選項](ValueSet-assessment-side-valueset.md) | 受試者評估側別選項 |
| [身體部位與結構對應之Snomed CT 代碼](ValueSet-VSBodyStructure.md) | 收錄復健可能會使用到的身體部位代碼 |
| [進食-選項](ValueSet-VSBarthelFeeding.md) |  |

### Terminology: Code Systems 

These define new code systems used by systems conforming to this implementation guide.

| |
| :--- |
| [CSMAS](CodeSystem-mas-score.md) |

### Example: Example Instances 

These are example instances that show what data produced and consumed by systems conforming with this implementation guide might look like.

| | |
| :--- | :--- |
| [ARAT問卷回覆範例](QuestionnaireResponse-arat-response-example-001.md) | 一位中風患者進行ARAT上肢功能評估的完整問卷回覆範例，包含所有測試項目分數、完成時間及自動計算總分 |
| [ARAT評估Bundle範例](Bundle-arat-bundle-001.md) | 包含患者、治療師及問卷回覆的完整評估資料包 |
| [ARAT評估會期](Encounter-arat-assessment-encounter-001.md) | 進行ARAT評估的門診會期 |
| [BBTExample](QuestionnaireResponse-BBTExample.md) |  |
| [BarthelIndexExample](QuestionnaireResponse-BarthelIndexExample.md) |  |
| [Fugl-Meyer上肢動作評估問卷回覆範例](QuestionnaireResponse-FMAUEMotorQuestionnaireResponseExample.md) | 針對 Fugl-Meyer 上肢動作評估問卷的完整回覆範例，展示左側上肢動作功能評估結果 |
| [Fugl-Meyer上肢感覺評估問卷回覆範例](QuestionnaireResponse-FMAUESensoryQuestionnaireResponseExample.md) | 針對Fugl-Meyer上肢感覺評估問卷的完整回覆範例 |
| [IDALQuestionnaireResponseInstance](QuestionnaireResponse-IDALQuestionnaireResponseInstance.md) |  |
| [MASQuestionnaireResponseExample](QuestionnaireResponse-MASQuestionnaireResponseExample.md) |  |
| [MMSEQuestionnaireResponseExample](QuestionnaireResponse-MMSEQuestionnaireResponseExample.md) |  |
| [MRCQuestionnaireResponseExample](QuestionnaireResponse-MRCQuestionnaireResponseExample.md) |  |
| [PAC照護計畫資料範例](CarePlan-PACCarePlanExample.md) | 一個照護計畫的範例 |
| [PAC用藥資料範例](MedicationAdministration-PACMedicationAdministrationExample.md) | 一個用藥資料的範例 |
| [WMFT上肢功能評估問卷回覆範例](QuestionnaireResponse-WMFTQuestionnaireResponseExample.md) | 針對 WMFT 上肢功能評估問卷的完整回覆範例，展示右側上肢功能評估結果，包含功能評分與完成時間記錄 |
| [中風患者範例](Patient-stroke-patient-001.md) | 右側中風患者，接受左側上肢功能評估 |
| [介入資料範例](Procedure-ProcedureExample.md) | 一個介入的範例 |
| [健康照護服務提供者角色資料範例](PractitionerRole-PractitionerRoleExample.md) | 一名健康照護服務提供者角色的範例 |
| [健康狀態篩檢與評估範例](Observation-ObservationScreeningAssessmentExample.md) | 一個健康狀態篩檢與評估的範例 |
| [復健治療師範例](Practitioner-ot-therapist-001.md) | 執行ARAT評估的職能治療師 |
| [機構資料範例](Organization-OrganizationExample.md) | 一個機構的範例 |
| [照護計畫資料範例](CarePlan-CarePlanExample.md) | 一個照護計畫的範例 |
| [用藥資料範例](MedicationAdministration-MyMedicationAdministrationExample.md) | 一個用藥資料的範例 |
| [目標資料範例](Goal-GoalExample.md) | 一個目標的範例 |

