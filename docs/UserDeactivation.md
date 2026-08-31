# Dora.UserDeactivation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**deactivationId** | **String** |  | 
**userId** | **String** |  | 
**requestedBy** | **String** | Admin that requested the deactivation. | 
**reason** | **String** |  | 
**status** | **String** | PENDING: wind-down in progress. FAILED: wind-down gave up; admin can re-trigger. COMPLETED: account deactivated. REACTIVATED: blocks lifted. | 
**attempts** | **Number** | Wind-down attempts performed so far. | 
**result** | **String** | Latest wind-down outcome or error summary. | [optional] 
**createdAt** | **Date** |  | 
**updatedAt** | **Date** |  | 
**completedAt** | **Date** |  | [optional] 
**reactivatedBy** | **String** |  | [optional] 
**reactivatedAt** | **Date** |  | [optional] 



## Enum: StatusEnum


* `PENDING` (value: `"PENDING"`)

* `FAILED` (value: `"FAILED"`)

* `COMPLETED` (value: `"COMPLETED"`)

* `REACTIVATED` (value: `"REACTIVATED"`)




