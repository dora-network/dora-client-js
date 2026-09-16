# Dora.IssuePromoLinkBatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sourceType** | [**PromoSourceType**](PromoSourceType.md) |  | 
**sourceId** | **String** |  | 
**sourceName** | **String** |  | [optional] 
**allocation** | **Number** | Cannot exceed the configured max_links_per_batch or remaining campaign capacity. | 
**note** | **String** |  | [optional] 
**expiresAt** | **Date** | Defaults to challenge end and must fall between challenge start and end in the future. | [optional] 


