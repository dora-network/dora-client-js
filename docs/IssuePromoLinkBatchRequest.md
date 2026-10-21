# Dora.IssuePromoLinkBatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sourceType** | [**PromoSourceType**](PromoSourceType.md) |  | 
**sourceId** | **String** |  | 
**sourceName** | **String** |  | [optional] 
**allocation** | **Number** | Required for SINGLE_USE; omit for REUSABLE. Bounded by max_links_per_batch. Minting reserves no campaign place. | [optional] 
**note** | **String** |  | [optional] 
**expiresAt** | **Date** | Defaults to challenge end and must fall between challenge start and end in the future. | [optional] 
**linkType** | **String** | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. | [optional] 
**affiliateProgramId** | **String** |  | [optional] 
**affiliateMemberId** | **String** | Existing affiliate referrer/member ID, not user ID. | [optional] 
**referralCode** | **String** | An existing code belonging to the selected member. Required with both IDs for reusable links; bound on the server and revalidated at claim time. | [optional] 



## Enum: LinkTypeEnum


* `SINGLE_USE` (value: `"SINGLE_USE"`)

* `REUSABLE` (value: `"REUSABLE"`)




