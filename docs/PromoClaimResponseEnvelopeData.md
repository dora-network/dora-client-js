# Dora.PromoClaimResponseEnvelopeData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**state** | [**PromoClaimState**](PromoClaimState.md) |  | 
**email** | **String** |  | [optional] 
**campaignName** | **String** |  | [optional] 
**promoCredit** | **String** |  | [optional] 
**minRewardAmount** | **String** |  | [optional] 
**maxRewardAmount** | **String** |  | [optional] 
**targetEquity** | **String** |  | [optional] 
**expiresAt** | **Date** |  | [optional] 
**sourceName** | **String** |  | [optional] 
**linkType** | **String** | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. | [optional] 
**affiliateProgramId** | **String** |  | [optional] 
**affiliateMemberId** | **String** | Existing affiliate referrer/member ID, not user ID. | [optional] 
**referralCode** | **String** | An existing code belonging to the selected member. Required with both IDs for reusable links; bound on the server and revalidated at claim time. | [optional] 
**campaignId** | **String** |  | [optional] 
**linkId** | **String** |  | [optional] 
**sourceId** | **String** |  | [optional] 



## Enum: LinkTypeEnum


* `SINGLE_USE` (value: `"SINGLE_USE"`)

* `REUSABLE` (value: `"REUSABLE"`)




