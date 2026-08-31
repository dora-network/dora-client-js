# Dora.TradingChallengeRegistrationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** |  | 
**tradingChallengeId** | **String** |  | 
**tradingChallengeName** | **String** |  | [optional] 
**tradingChallengeType** | **String** |  | [optional] 
**tradingChallengeStatus** | **String** |  | [optional] 
**userId** | **String** |  | 
**userEmail** | **String** |  | [optional] 
**userName** | **String** |  | [optional] 
**tenantId** | **String** |  | 
**status** | **String** |  | 
**reviewedBy** | **String** | Who settled the request. Absent while it is PENDING. | [optional] 
**reviewedAt** | **Date** | When it was settled. Absent while it is PENDING. | [optional] 
**reviewReason** | **String** | Free-text note kept for the audit trail. Optional on both decisions. | [optional] 
**createdAt** | **Date** |  | 
**updatedAt** | **Date** |  | 



## Enum: TradingChallengeTypeEnum


* `TOURNAMENT` (value: `"TOURNAMENT"`)

* `CASH` (value: `"CASH"`)





## Enum: TradingChallengeStatusEnum


* `PENDING` (value: `"PENDING"`)

* `ACTIVE` (value: `"ACTIVE"`)

* `COMPLETED` (value: `"COMPLETED"`)





## Enum: StatusEnum


* `PENDING` (value: `"PENDING"`)

* `APPROVED` (value: `"APPROVED"`)

* `REJECTED` (value: `"REJECTED"`)




