# Dora.IssuePromoLinkBatchResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**batchId** | **String** |  | 
**sourceId** | **String** |  | 
**allocation** | **Number** |  | [optional] 
**links** | [**[IssuedPromoLink]**](IssuedPromoLink.md) |  | 
**linkType** | **String** | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. | [optional] 
**affiliateProgramId** | **String** |  | [optional] 
**affiliateMemberId** | **String** | Existing affiliate referrer/member ID, not user ID. | [optional] 
**referralCode** | **String** | An existing code belonging to the selected member. Required with both IDs for reusable links; bound on the server and revalidated at claim time. | [optional] 



## Enum: LinkTypeEnum


* `SINGLE_USE` (value: `"SINGLE_USE"`)

* `REUSABLE` (value: `"REUSABLE"`)




