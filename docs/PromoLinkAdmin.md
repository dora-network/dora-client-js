# Dora.PromoLinkAdmin

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** |  | 
**tokenPrefix** | **String** |  | 
**url** | **String** | Only present when reveal&#x3D;true. Private; do not log or cache. | [optional] 
**status** | **String** | Reusable links use ACTIVE or REVOKED and have no single claimant. | 
**expiresAt** | **Date** |  | 
**claimedAt** | **Date** |  | [optional] 
**claimedEmail** | **String** | Masked as the first character, three asterisks, and domain. | [optional] 
**userId** | **String** |  | [optional] 
**linkType** | **String** | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. | [optional] 



## Enum: StatusEnum


* `ISSUED` (value: `"ISSUED"`)

* `CLAIMED` (value: `"CLAIMED"`)

* `REVOKED` (value: `"REVOKED"`)

* `ACTIVE` (value: `"ACTIVE"`)





## Enum: LinkTypeEnum


* `SINGLE_USE` (value: `"SINGLE_USE"`)

* `REUSABLE` (value: `"REUSABLE"`)




