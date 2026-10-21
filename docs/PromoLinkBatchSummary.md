# Dora.PromoLinkBatchSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** |  | 
**sourceType** | [**PromoSourceType**](PromoSourceType.md) |  | 
**sourceId** | **String** |  | 
**sourceName** | **String** |  | 
**allocation** | **Number** |  | [optional] 
**issued** | **Number** |  | [optional] 
**claimed** | **Number** |  | [optional] 
**revoked** | **Number** |  | [optional] 
**createdAt** | **Date** |  | 
**linkType** | **String** | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. | [optional] 
**affiliateProgramId** | **String** |  | [optional] 
**affiliateMemberId** | **String** | Existing affiliate referrer/member ID, not user ID. | [optional] 
**referralCode** | **String** | An existing code belonging to the selected member. Required with both IDs for reusable links; bound on the server and revalidated at claim time. | [optional] 
**campaignId** | **String** |  | [optional] 
**signups** | **Number** | Successful signups; reusable links omit allocation/issued/claimed/revoked counts. | [optional] 



## Enum: LinkTypeEnum


* `SINGLE_USE` (value: `"SINGLE_USE"`)

* `REUSABLE` (value: `"REUSABLE"`)




